# Prüfen

### Beschreibung

{% hint style="warning" %}
Dies ist eine **Methode** oder ein **Unterbefehl** des Befehls [Config](./). Es ist kein eigener Befehl.
{% endhint %}

Diese Methode des [Konfigurations](./)-Befehls kann verwendet werden, um zu überprüfen, ob Sie alle Ihre Konfigurationsschlüssel richtig eingegeben haben. Der Befehl antwortet mit einer Einbettung, die den Schlüsselnamen und die Werten enthalten, auf den sie eingestellt sing.

Wenn kein Schlüssel gesetzt ist, wird ein "No Sign"-Emoji anziegen.  
Wenn ein **set** Schlüssel richtig konfiguriert ist, zeigt es den Wert an, auf den es eingestellt wurde.  
Einige  **set** Schlüssel sind auf einen Standardwert konfiguriert, der auch im Prüfbefehl angezeigt wird.  
Wenn ein **toggle** Schlüssel auf "true" gesetzt ist, wird ein "Yes-Sign"-Emoji angezeigt, und wenn sie auf "false" gesetzt ist, wird ein "No-Sign"-Emoji angezeigt.

### Befehlsstruktur

```text
p!config check
```

Nachfolgend finden Sie eine Tabelle mit allen Konfigurationsschlüsseln, die in der Prüfmethode angezeigt werden, zusammen mit allen Standardwerten.

| Schlüssel | Standardprüfwert |
| :--- | :--- |
| Meilenstein-Kanal | ❌ \(Nicht Eingestellt\) |
| Meilensteinintervall | ✅ \(100\) |
| Präfix | ✅ \(p!\) |
| Mitgliederzahl | ✅ \(An\) |
| Automatische Rolle | ❌ \(Nicht Eingestellt\) |
| Automatisches Rollen Timeout | ❌ \(Nicht Eingestellt\) |
| Emoji-Liste | ❌ \(Nicht Eingestellt\) |
| Kanäle auf der schwarzen Liste | ❌ \(Nicht Eingestellt\) |
| XP Kanäle  | ❌ \(Nicht Eingestellt\) |
| XP Rollen | ❌ \(\(Nicht Eingestellt\) |
| Stapeln von XP Rollen | ✅ \(Wahr\) |
| Top XP Rolle | ❌ \(Nicht Eingestellt\) |
| Keine XP Rollen | ❌ \(Nicht Eingestellt\) |
| Automatisch veröffentliche Kanäle | ❌ \(Nicht Eingestellt\) |
| Abklingzeit der Rollenerwähnung | ✅ \(0ms\) |
| Erwähnte Abklingzeitrollen | ❌ \(Nicht Eingestellt\) |
| XP Antworttyp | ✅ \(Derselbe Kanal\) |
| XP Benachrichtigung | ✅ \({user} has reached level **{level}**\) |
| Meilenstein-Nachricht | ✅ \(**{milestone} Members**  Congratulations to {user}, you were the {milestone}th person to join!\) |

### **Berechtigungen**

* `Server verwalten`**\(Benutzer\)**
* N/A **\(Bot\)**

### Aliase

* N/A



