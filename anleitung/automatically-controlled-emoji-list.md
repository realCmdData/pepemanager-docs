---
description: >-
  Richten Sie eine Liste aller Ihrer Server-Emojis ein und vergessen Sie sie, da
  sie sich selbst aktualisiert!
---

# Automatisch gesteuerte Emoji-Liste

### Warum sollten Sie das brauchen?

Ein wesentliches Feature von Discord Emoji Servern sind die komfortabel erstellten Emoji-Listen. Herkömmlicherweise sind sie ein Kanal, der der Auflistung aller Emojis gewidmet ist, die sich auf einem Server oder in einigen Fällen auf einer Vielzahl von Servern befinden, sodass Benutzer ihre Favoriten einfach kopieren und einfügen können, nach verlockenden Emojis suchen und mehr.  
Pepe Manager bietet genau dies an, und gibt Ihnen die Freiheit ihn einzurichten und zu vergessen, da er die gesamte Arbeit im Hintergrund erledigt.

### Videoanleitung

Wenn Sie langes Lesen abgeneigt sind, haben wir ein Video-Tutorial erstellt, das leicht zu verstehen sein sollte:

**\(NUR AUF ENGLISCH ERHÄLTLICH\)**

{% embed url="https://youtube.com/watch?v=CYMIeDcgeek" %}

## Anleitung

### Einstellen des Kanals

Als erstes möchten Sie einen Kanal für Ihre Emoji-Liste erstellen. Dies wird der endgültiger Kanal für die Liste sein, also richten Sie ihn so ein das später alle ihn sehen können.

Als nächstes möchten Sie den folgenden Befehl eingeben:

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set emojiListChannel <Channel/ChannelID/ChannelMention>
```

{% hint style="info" %}
Sie können den Kanal einstellen, indem Sie den Namen des Kanals schreiben, die Kanal-ID verwenden oder einfach den Kanal erwähnen. Wenn Sie einen unvollständigen Kanalnamen eingeben, sucht der Bot nach dem nächstgelegenen.
{% endhint %}

### Aktivieren der Liste

Als nächstes möchten Sie die Emoji-Liste aktivieren. Selbst wenn Sie den emojiListChannel eingestellt haben, ist er standardmäßig nicht aktiviert. Geben Sie zum Aktivieren den folgenden Befehl ein:

```text
p!config toggle emojiList
```

### Aktualisieren der Liste

Schließlich müssen Sie die Emoji-Liste manuell aktualisieren, um Ihre neue Emoji-Liste in Gang zu bringen. Dies ist das einzige Mal, dass Sie es manuell aktualisieren müssen, Sie können die Liste jedoch später jederzeit manuell aktualisieren:

```text
p!updateemojilist
```

### Letzte Worte

Und das ist alles! Sie haben mit Pepe Manager erfolgreich eine automatisch gesteuerte Emoji-Liste erstellt!

Die Emoji-Liste wird bei diesen Ereignissen automatisch aktualisiert:

* Ein Emoji wird erstellt
* Ein Emoji wird gelöscht
* Ein Emoji wird umbenannt
* Ein Emoji wird ersetzt \(mit Pepe Manager-Befehlen\)

Wenn Sie weitere Hilfe zu Pepe Manager benötigen, lesen Sie den Rest dieser Dokumentation oder treten Sie unserem Support-Server bei, um mit einem echten Menschen zu sprechen!



### 

