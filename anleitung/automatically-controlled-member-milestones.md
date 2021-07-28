---
description: >-
  Erfahren Sie, wie Pepe Manager automatisch einen Meilenstein mit Ihnen feiern
  kann!
---

# Automatisch kontrollierte Mitglieder-Meilensteine

### Warum sollten Sie das brauchen?

Einen Mitglieder-Meilenstein zu feiern ist eine super einfache und soziale Aktivität. Ob Sie 100 oder 100.000 Mitglieder feiern, es ist ein ebenso bedeutsamer Anlass wie jeder andere. Indem Sie den Benutzer, der als Ihr n-tes Mitglied beigetreten ist, feiern und belohnen, können Sie sich immer ein neues Ziel setzen, ein neues Wachstumsniveau erreichen. Die Automatisierung dieses Prozesses ist schnell und einfach, und die Möglichkeiten sind endlos!

### Videoanleitung

Wenn Sie langes Lesen abgeneigt sind, haben wir ein Video-Tutorial erstellt, das leicht zu verstehen sein sollte:

**\(NUR AUF ENGLISCH ERHÄLTLICH\)**

{% embed url="https://youtu.be/nXlhdcH3YaU" %}

## Anleitung

### Meilensteine aktivieren

Der erste Schritt besteht darin, die Meilensteinfunktion in Ihren Pepe Manager-Einstellungen zu aktivieren. Dies ist ein nützlicher Schalter, wenn Sie keine Meilensteine mehr verwenden möchten, aber alle Ihre konfigurierten Einstellungen behalten möchten, auf die wir später eingehen werden. Um es zu aktivieren, geben Sie den folgenden Befehl ein:

```text
p!config toggle milestones
```

### Einstellen des Meilenstein-Kanals

Der nächste Schritt besteht darin, einen Meilenstein-Kanal einzurichten, in den alle Ihre automatisierten Meilenstein-Ankündigungen gesendet werden! Dies kann ein normaler Textkanal sein, oder wenn Sie einen Community-Enabled-Server haben, kann dies auch ein Ankündigungskanal sein. Geben Sie den folgenden Befehl ein, um Ihren Kanal einzurichten:

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set milestonesChannel <Channel/ChannelID/ChannelMention>
```

### Einstellen des Meilensteinintervalls

Dieser nächste Schritt ist sehr wichtig, denn jetzt können Sie auswählen, bei welcher Mitgliederzahl Ihr Meilenstein ausgelöst werden soll. Das Intervall ist die Anzahl der Mitglieder zwischen jedem Meilenstein und ist standardmäßig auf **100** eingestellt. Dies bedeutet, dass alle **100** Mitglieder ein Meilenstein ausgelöst wird, z. B. **200**, **300**, **400** usw.

Das Meilensteinintervall kann eine beliebige Zahl innerhalb eines vernünftigen Rahmens sein, solange es ein _**Vielfaches von 5**_ ist. Denkbar ist, dass das Intervall auf **5** oder auf **100.000** gesetzt werden kann. Geben Sie den folgenden Befehl ein, um Ihr Intervall festzulegen:

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set milestonesInterval <Number>
```

### Einstellen der Meilenstein-Nachricht

Als nächstes können Sie auch Ihre Meilensteinnachricht anpassen, die gesendet wird, wenn ein Meilenstein erreicht wird. Standardmäßig sieht die Nachricht wie folgt aus:

![](https://i.imgur.com/IUZMJGP.png)

Sie können eine beliebige Anzahl von Emojis \(solange der Bot darauf zugreifen kann\), Formatierungen, Zeilenumbrüche, Sonderzeichen und sogar Rollenerwähnungen einfügen, solange dies innerhalb der 2000-Zeichen-Grenze aller Nachrichten liegt. Geben Sie den folgenden Befehl ein, um Ihre Meilensteinnachricht festzulegen:

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set milestonesMessage <Message>
```

{% hint style="warning" %}
Wenn Sie eine Rollenerwähnung in Ihre Nachricht einfügen, stellen Sie sicher, dass Pepe Manager die Berechtigung hat, diese Rolle zu erwähnen, da es sonst nicht richtig funktionieren wird.
{% endhint %}

Es gibt mehrere Tags, die Sie in Ihre Milestone-Nachricht einfügen können. Diese Parameter werden beim Senden der Milestone-Nachricht durch die entsprechenden Informationen ersetzt.  
  
_Sie müssen die Klammern {} in Ihre Nachricht einfügen, damit die Tags angezeigt werden!_

| Information | Tag |
| :--- | :--- |
| Benutzter Erwähnung \(@User\) | {user} |
| Benutzter Tag \(User\#1234\) | {user.tag} |
| Benutzter Name \(User\) | {user.username\) |
| Benutzter Diskriminator \(1234\) | {user.discriminator} |
| Benutzter ID \(99787644430475264\) | {user.id} |
| Server Name \(My Cool Server\) | {guild.name} |
| Server ID \(493351982887862283\) | {guild.id} |
| Meilenstein Erreicht \(100\) | {milestone} |

### Festlegen der Meilenstein-Rolle

Schließlich können Sie auch Benutzer, die zum richtigen Zeitpunkt beigetreten sind, belohnen, indem Sie ihnen eine oder mehrere Rollen zuweisen. Kostenlose Server können bis zu **5** Rollen einrichten, die an diese besondere Person vergeben werden, und [Premium-Server](../information/patreon-perks.md) können bis zu **10** Rollen einrichten. Geben Sie den folgenden Befehl ein, um Ihre Meilensteinrolle\(n\) festzulegen:

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set milestonesRole <Role/RoleID/RoleMention>
```

### Letzte Worte

Und das ist es! Sie haben die Automatisch kontrollierten Mitglieder-Meilensteine mit Pepe Manager erfolgreich erstellt!

Wenn Sie weitere Hilfe zu Pepe Manager benötigen, lesen Sie den Rest dieser Dokumentation oder treten Sie unserem Support-Server bei, um mit einem echten Menschen zu sprechen!

