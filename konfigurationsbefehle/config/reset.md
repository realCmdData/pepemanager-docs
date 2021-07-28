# Zurücksetzen

### Beschreibung

{% hint style="warning" %}
Dies ist eine **Methode** oder ein **Unterbefehl** des Befehls [Config](./). Es ist kein eigener Befehl.
{% endhint %}

Diese Methode des [Config ](./)Befehls kann verwendet werden, um die [Toggle ](toggle.md)Schlüssel auf ihren Standardzustand zurückzusetzen.

Die Reset-Methode funktioniert nicht bei gesetzten Schlüsseln, bitte beachten Sie die [Lösch](delete.md)-Methode!

### Befehlsstruktur

Wobei **&lt; &gt;** ein erforderlicher Parameter ist

```text
p!config reset <Key>
```

| Schlüssel | Beschreibung | Status beim Zurücksetzen |
| :--- | :--- | :--- |
| counts | Steuert, ob der Bot Mitglieder beim beitritt und verlassen Zählt | ❌ \(Aus\) |
| emojiList | Steuert, ob die Emoji-Listenfunktion aktiviert ist oder nicht | ❌ \(Aus\) |
| levels | Steuert, ob die Leveling-funktion aktiviert ist oder nicht | ❌ \(Aus\) |
| milestones | Steuert, ob die Meilensteinfunktion aktiviert ist oder nicht | ❌ \(Aus\) |
| stackXpRoles | Steuert, ob [Rollenbelohnungen ](../../anleitung/setting-up-server-xp-leveling.md#hinzufuegen-von-rollenbelohnungen)gestapelt werden oder nicht | ✅ \(Stapelbar\) |

### **Berechtigungen**

* `Server verwalten`**\(Benuzter\)**
* N/A **\(Bot\)**

### Aliase

* N/A



