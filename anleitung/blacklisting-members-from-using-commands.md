---
description: 'Erfahren Sie, wie Sie Pepe Manager auf bestimmte Kanäle beschränken!'
---

# Kanäle auf die schwarze Liste setzen

### Warum sollten Sie das brauchen?

Einen Server zu moderieren ist schon schwieriger als nötig. Und es ist auch schwierig, alle Bots auf einen oder mehrere Kanäle zu beschränken, um Benutzer daran zu hindern, sie in allgemeinen Kanälen zu verwenden und/oder zu missbrauchen. Der einfachste Weg, alles dort zu behalten, wo es sein soll, ist das Blacklisting. Lassen Sie Pepe Manager nur in bestimmten Bereichen auf Befehle reagiere!

### Videoanleitung

Wir haben derzeit noch kein Video-Tutorial für diese Anleitung, schauen Sie später noch einmal vorbei!

## Anleitung

### Verstehen, wie die Blacklist funktioniert

Einen Kanal mit Pepe Manager auf die schwarze Liste zu setzen ist ähnlich wie die einfache Verwendung von Berechtigungen, um einzuschränken, wer Befehle in welchem Kanal verwenden kann. Mit Pepe Manager ist es jedoch viel einfacher zu tun.

Wenn ein Kanal auf die schwarze Liste gesetzt wird, können alle Mitglieder, die regelmäßig in diesem Kanal chatten können, keine Pepe Manager-Befehle mehr ausführen. Dies gilt jedoch nicht für Serveradministratoren, dh. jeder mit der Admin-Berechtigung.

{% hint style="warning" %}
Wenn Sie über die Admin-Berechtigung verfügen, umgehen Sie die Blacklist, auch wenn sie wie vorgesehen funktioniert.
{% endhint %}

### Kanäle auf die schwarze Liste setzen

Um Kanäle zur Blacklist hinzuzufügen, können Sie den folgenden Befehl ausführen, einschließlich beliebig vieler Kanäle. Sie können später jederzeit weitere Kanäle hinzufügen, wenn Sie möchten, und Sie können Kanäle auch nach Belieben löschen.

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set blacklistedChannels <Channel/ChannelID/ChannelMention>
```

### Kanäle von der schwarzen Liste entfernen

Das Entfernen von Kanälen von der Blacklist ist fast so einfach wie das Hinzufügen, nur umgekehrt! Denken Sie natürlich daran, dass ein Kanal zum Entfernen von der Blacklist zuerst auf dem enthalten sein muss. Um einen oder mehrere Kanäle aus der Blacklist zu entfernen, führen Sie den folgenden Befehl aus:

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config delete blacklistedChannels <Channel/ChannelID/ChannelMention>
```

### Letzte Worte

Und das ist alles! Sie haben erfolgreich gelernt, wie Sie Kanäle auf der schwarzen Liste von Pepe Manager hinzufügen und entfernen, um Ihren Server effizienter zu verwalten! 

Wenn Sie weitere Hilfe zu Pepe Manager benötigen, lesen Sie den Rest dieser Dokumentation oder treten Sie unserem Support-Server bei, um mit einem echten Menschen zu sprechen!

