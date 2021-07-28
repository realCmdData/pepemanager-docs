---
description: >-
  Erfahren Sie, wie Sie Ankündigungskanäle einrichten, um Nachrichten
  automatisch zu veröffentlichen!
---

# Ankündigungen automatisch veröffentlichen

### Warum sollten Sie das brauchen?

Wenn Sie noch nie von ihnen gehört haben, sind [Discord-Ankündigungskanäle](https://support.discord.com/hc/de/articles/360032008192-Announcement-Channels-) eine äußerst nützliche Ergänzung zu jedem Community-Server, um ihre Reichweite auf ein Publikum außerhalb Ihres eigenen Servers auszudehnen! Aber dazu müssen Sie manuell auf einen kleinen Knopf klicken, um sicherzustellen, dass die Ankündigung auch auf alle Ihre folgenden Server gepusht wird, und ohne Zweifel haben Sie manchmal einfach vergessen, diesen Knopf zu klicken! 

Nun, mit Pepe Manager können Sie es so einrichten, dass ein Ankündigungskanal alle Ankündigungen, die Sie an den Kanal senden, automatisch ausstößt!

### Videoanleitung

Wenn Sie langes Lesen abgeneigt sind, haben wir ein Video-Tutorial erstellt, das leicht zu verstehen sein sollte:

**\(NUR AUF ENGLISCH ERHÄLTLICH\)**

{% embed url="https://youtu.be/d6\_HNHrJ8lU" %}

## Anleitung

### Erstellen eines Ankündigungskanals

Der erste Schritt zum Erstellen eines Ankündigungskanals besteht darin, die Community-Serverfunktionen zu aktivieren, indem Sie dieser [Anleitung ](https://support.discord.com/hc/de/articles/360047132851-Enabling-Your-Community-Server)von Discord selbst folgen!

Der nächste Schritt besteht darin, einen neuen Kanal zu erstellen und als Kanaltyp auszuwählen: 'Ankündigungskanal'. Geben Sie ihm einen passenden Namen und fahren Sie dann mit dem nächsten Schritt fort!

![](../.gitbook/assets/kzgyljb.png)

### Berechtigungen erteilen

Dieser nächste Schritt ist ganz entscheidend. Standardmäßig kann Pepe Manager keine Nachrichten im neuen Kanal ankündigen. Daher müssen Sie entweder Pepe Manager \(Den Bot Account\) oder Pepe Manager \(Die Integrations Rolle\) die Berechtigung zum Senden von Nachrichten in dem neu erstellten Ankündigungskanal.

{% hint style="info" %}
Keine Sorge, der Bot wird niemals von sich aus Nachrichten in Ihren Ankündigungskanal senden, er benötigt diese Berechtigung nur, um bereits gesendete Nachrichten anzukündigen.
{% endhint %}

![](../.gitbook/assets/ligkvrd.png)

### Konfigurieren des Automatischen Veröffentlichers

Schließlich müssen wir Pepe Manager mitteilen, welcher Ankündigungskanal automatisch veröffentlicht werden soll! Standardmäßig können kostenlose Server bis zu 5 separate automatische Ankündigungskanäle einrichten, [Premium](../information/patreon-perks.md)-Server können jedoch bis zu 25 automatische Ankündigungskanäle einrichten. Geben Sie den folgenden Befehl ein, um zu beginnen:

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set autoPublishChannels <Channel/ChannelID/ChannelMention>
```

### Letzte Worte

Und das ist alles! Sie haben mit Pepe Manager erfolgreich einen automatisch veröffentlichenden Ankündigungskanal erstellt! 

Wenn Sie weitere Hilfe zu Pepe Manager benötigen, lesen Sie den Rest dieser Dokumentation oder treten Sie unserem Support-Server bei, um mit einem echten Menschen zu sprechen!

