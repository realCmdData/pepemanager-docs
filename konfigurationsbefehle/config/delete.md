# Löschen

### Beschreibung

{% hint style="warning" %}
Dies ist eine **Methode** oder ein **Unterbefehl** des Befehls [Config](./). Es ist kein eigener Befehl.
{% endhint %}

Diese Methode des [Configs](./)-Befehl kann verwendet werden, um die unten aufgeführten Schlüssel zu löschen. Sobald ein Schlüssel gelöscht wurde, kann er nicht wiederhergestellt werden und muss manuell neu gesetzt werden.

Die Löschmethode funktioniert nicht bei **toggle** Schlüsseln, bitte beachten Sie die [Reset](reset.md)-Methode!

### Befehlsstruktur

Wobei **&lt; &gt;** ein erforderlicher Parameter ist

```text
p!config delete <Key>
```

| Schlüssel | Beschreibung |
| :--- | :--- |
| autoPublishChannels | [Ankündigungskanäle](https://support.discord.com/hc/de/articles/360032008192-Announcement-Channels-), die Sie automatisch veröffentlichen möchten |
| autoResetLevels | Setzt Benutzer-Levels automatisch zurück, wenn die von Ihnen festgelegten Bedingungen erfüllt sind |
| autoRole | Rollen, die Sie neuen Mitgliedern automatisch zuweisen möchten |
| autoRoleTimeout | Zeitspanne zwischen dem Beitritt eines Benutzers und dem Erhalt einer Rolle |
| blacklistedChannels | Kanäle, in denen Pepe Manager-Befehle nicht funktionieren |
| emojiListChannel | Der Kanal für die automatisierte Emoji-Liste |
| mentionCooldown | Zeitspanne zwischen Rollenerwähnungen |
| mentionCooldownRoles | Erwähnbare Rollen, für die Sie eine Erwähn-Abklingzeit haben möchten |
| milestonesChannel | Der Kanal für alle Meilenstein-Ankündigungen |
| milestonesInterval | Die Anzahl der Mitglieder zwischen den Meilensteinen |
| milestonesMessage | Die Nachricht, die gesendet wird, wenn ein Meilenstein erreicht ist |
| milestonesRole | Die Rolle\(n\), die der Person zugewiesen wird, die bei Erreichen des Meilensteins beitritt |
| noXpRoles | Rollen, die auf dem gesamten Server kein XP erhalten sollen |
| prefix | Das Server-Präfix, das der Bot verwenden soll \(Standard ist p!\) |
| topXpRole | Die Rolle, die Sie dem Benutzer geben möchten, der an diesem Tag die Bestenliste führt |
| xpBlacklistedChannels | Kanäle, in denen **kein** XP erhalten werden soll. Alle anderen Kanäle können XP erhalten |
| xpMessage | Die Nachricht, die gesendet wird, wenn jemand hoch-leveled. |
| xpMultiplier | Stellen Sie verschiedene Multiplikatoren für den variablen XP Gewinn ein |
| xpResponseType | Das Ziel jeder Level-Up-Nachricht |
| xpRoles | Rollenbelohnungen, die Sie an einem bestimmten Level ausgeben möchten |
| xpWhitelistedChannels | Kanäle, in denen Sie XP erhalten **möchten**. Alle anderen Kanäle können kein XP erhalten |

### **Berechtigungen**

* `Server verwalten`**\(Benutzer\)**
* N/A **\(Bot\)**

### Aliase

* `del`
* `remove`
* `rm`



