# Setzen

### Beschreibung

{% hint style="warning" %}
Dies ist eine **Methode** oder ein **Unterbefehl** des Befehls [Config](./). Es ist kein eigener Befehl.
{% endhint %}

Diese Methode des [Config ](./)Befehls kann verwendet werden, um die unten aufgeführten Schlüssel festzulegen. Der Wert, auf den Sie Schlüssel einstellen können, hängt davon ab, welchen Schlüssel Sie festlegen möchten.

### Befehlsstruktur

Wobei **&lt; &gt;** ein erforderlicher Parameter ist

```text
p!config set <Key> <Value>
```

| Schlüssel | Beschreibung | Akzeptierter Wert |
| :--- | :--- | :--- |
| autoPublishChannels | [Ankündigungskanäle](https://support.discord.com/hc/de/articles/360032008192-Announcement-Channels-), die Sie automatisch veröffentlichen möchten | Kanäle |
| autoResetLevels | Setzt Benutzer-Levels automatisch zurück, wenn die von Ihnen festgelegten Bedingungen erfüllt sind | [See Here](https://docs.pepemanager.com/v/deutsch/anleitung/setting-up-server-xp-leveling#levels-automatisch-zuruecksetzen) |
| autoRole | Rollen, die Sie neuen Mitgliedern automatisch zuweisen möchten | Rollen |
| autoRoleTimeout | Zeitspanne zwischen dem Beitritt eines Benutzers und dem Erhalt einer Rolle | Zeitintervall |
| blacklistedChannels | Kanäle, in denen Pepe Manager-Befehle nicht funktionieren | Kanäle |
| emojiListChannel | Der Kanal für die automatisierte Emoji-Liste | Kanal |
| mentionCooldown | Zeitspanne zwischen Rollenerwähnungen | Zeitintervall |
| mentionCooldownRoles | Erwähnbare Rollen, für die Sie eine Erwähn-Abklingzeit haben möchten | Rollen |
| milestonesChannel | Der Kanal für alle Meilenstein-Ankündigungen | Kanal |
| milestonesInterval | Die Anzahl der Mitglieder zwischen den Meilensteinen | Beliebiges Vielfaches von 5 |
| milestonesMessage | Die Nachricht, die gesendet wird, wenn ein Meilenstein erreicht ist | Nachricht |
| milestonesRole | Die Rolle\(n\), die der Person zugewiesen wird, die bei Erreichen des Meilensteins beitritt | Rollen |
| noXpRoles | Rollen, die auf dem gesamten Server kein XP erhalten sollen | Rollen |
| prefix | Das Server-Präfix, das der Bot verwenden soll \(Standard ist p!\) | Alphanumerische Werte und Symbole |
| topXpRole | Die Rolle, die Sie dem Benutzer geben möchten, der an diesem Tag die Bestenliste führt | Rolle |
| xpBlacklistedChannels | Kanäle, in denen **kein** XP erhalten werden soll. Alle anderen Kanäle können XP erhalten | Kanäle |
| xpMessage | Die Nachricht, die gesendet wird, wenn jemand hoch-leveled. | Nachricht |
| xpMultiplier | Stellen Sie verschiedene Multiplikatoren für den variablen XP Gewinn ein | [Siehe Hier](https://docs.pepemanager.com/v/deutsch/anleitung/setting-up-xp-multipliers) |
| xpResponseType | Das Ziel jeder Level-Up-Nachricht | [Siehe Hier](https://docs.pepemanager.com/v/deutsch/anleitung/setting-up-server-xp-leveling#wohin-die-level-up-nachricht-gesendet-werden-soll) |
| xpRoles | Rollenbelohnungen, die Sie an einem bestimmten Level ausgeben möchten | [Siehe Hier](https://docs.pepemanager.com/v/deutsch/anleitung/setting-up-server-xp-leveling#hinzufuegen-von-rollenbelohnungen) |
| xpWhitelistedChannels | Kanäle, in denen Sie XP erhalten **möchten**. Alle anderen Kanäle können kein XP erhalten | Kanäle |

### Wertestruktur

Unten finden Sie eine Tabelle, in der aufgeführt ist, was jeder der oben aufgeführten Werte im Detail akzeptiert.

<table>
  <thead>
    <tr>
      <th style="text-align:left">Akzeptierter Wert</th>
      <th style="text-align:left">Was es beinhaltet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Kan&#xE4;le</td>
      <td style="text-align:left">
        <p>&#x2022; Kanal-Erw&#xE4;hnungen (#Kanal)</p>
        <p>&#x2022; Kanal-Namen (Kanal)</p>
        <p>&#x2022; Kanal IDs (841218613380644914)</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Rollen</td>
      <td style="text-align:left">
        <p>&#x2022; Rollen-Erw&#xE4;hnungen (@Rolle)</p>
        <p>&#x2022; Rollen-Name (Rolle)</p>
        <p>&#x2022; Rollen IDs (493352184377901066)</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Zeitintervall</td>
      <td style="text-align:left">
        <p>&#x2022; 60 sekunden (60s)</p>
        <p>&#x2022; 1 minute (1m)</p>
        <p>&#x2022; 3 stunden (3h)</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Nachricht</td>
      <td style="text-align:left">&#x2022; Jede g&#xFC;ltige Discord-Nachricht</td>
    </tr>
    <tr>
      <td style="text-align:left">Beliebiges Vielfaches von 5</td>
      <td style="text-align:left">&#x2022; Jede Zahl, die ein Vielfaches von 5 ist (10, 15, 50, 10000, 750)</td>
    </tr>
    <tr>
      <td style="text-align:left">Alphanumerische Werte und Symbole</td>
      <td style="text-align:left">&#x2022; Jedes Zeichen, das entweder eine Zahl (1, 2, 3) oder ein Buchstabe
        (a, b, c) oder ein allgemeines Symbol (!, $, %) ist</td>
    </tr>
  </tbody>
</table>

### **Berechtigungen**

* `Server verwalten`**\(Benutzer\)**
* N/A **\(Bot\)**

### Aliase

* N/A



