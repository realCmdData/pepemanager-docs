# Umschalten

### Beschreibung

{% hint style="warning" %}
Dies ist eine **Methode** oder ein **Unterbefehl** des Befehls [Config](./). Es ist kein eigener Befehl.
{% endhint %}

Mit dieser Methode des [Config](./)-Befehls kann eine Reihe von Schlüsseln umgeschaltet werden, die unten aufgeführt sind. Diese Schlüssel sind Boolesche Schlüssel, d. h. sie können nur entweder ein- oder ausgeschaltet oder von einem Wert auf einen anderen gesetzt werden. Umschaltschlüssel werden meist verwendet, um bestimmte Funktionen von Pepe Manager ein- oder auszuschalten.

### Befehlsstruktur

Wobei **&lt; &gt;** ein erforderlicher Parameter ist

```text
p!config toggle <Key>
```

| Schlüssel | Beschreibung | Standardzustand |
| :--- | :--- | :--- |
| counts | Steuert, ob der Bot das Ein- und Austreten von Mitgliedern zählt | ✅ \(On\) |
| emojiList | Steuert, ob die Emoji-Listenfunktion eingeschaltet ist oder nicht | ❌ \(Off\) |
| levels | Steuert, ob die Leveling-funktion eingeschaltet ist oder nicht | ❌ \(Off\) |
| milestones | Steuert, ob die Meilensteinfunktion eingeschaltet ist oder nicht | ❌ \(Off\) |
| prioritiseMultiplierRoleHierarchy | Steuert, ob die [Rollenpriorisierung ](https://docs.pepemanager.com/v/deutsch/anleitung/setting-up-xp-multipliers#aendern-der-rollenmultiplikatorhierarchie)eingeschaltet ist oder nicht | ❌ \(Multiplier Value\) |
| stackXpRoles | Steuert, ob [Rollenbelohnungen ](https://docs.pepemanager.com/v/deutsch/anleitung/setting-up-server-xp-leveling#hinzufuegen-von-rollenbelohnungen)gestapelt werden oder nicht | ✅ \(Stackable\) |

### **Berechtigungen**

* `Server verwalten`**\(Benuzter\)**
* N/A **\(Bot\)**

### Aliase

* N/A



