---
description: >-
  Belohnen Sie die Aktivität Ihrer Benutzer mit Levels, Rollen Belohnungen und
  mehr!
---

# Einrichten von Server XP/Leveling

### Warum sollten Sie das brauchen?

Server Leveling ist eine super einfache und effektive Möglichkeit, Aktivität und Wachstum auf Ihrem Discord-Server sicherzustellen. Durch das Festlegen von Aktivitätszielen mit Belohnungen werden Benutzer dazu verleitet, den Chat am Laufen zu halten, um dieses von Ihnen gesetzte Ziel zu erreichen. Dieses Ziel kann so ziehmlich alles sein, von etwas so Einfachem und kostengünstigem wie einer Rollenbelohnung, die dem Benutzer eine besondere Berechtigung wie die Möglichkeit zum Senden von Bildern gewährt, bis hin zur Belohnung der aktivsten Benutzer in Ihrem Discord mit Nitro Geschenken!  
   
Pepe Manager bietet ein kostenloses und benutzerfreundliches XP- und Leveling-System, damit Sie die Benutzerverbindung hoch und die Kosten niedrig halten können!

### Videoanleitung

Wenn Sie langes Lesen abgeneigt sind, haben wir ein Video-Tutorial erstellt, das leicht zu verstehen sein sollte:

**\(NUR AUF ENGLISCH ERHÄLTLICH\)**

{% embed url="https://youtu.be/H-x3\_94-T8E" %}

## Anleitung

### Levels Einschalten

Standardmäßig ist in Pepe Manager die Leveling-funktion nicht aktiviert. Alle Benutzeraktivitäten, die möglicherweise vor der Aktivierung der Leveling-funktion aufgetreten sind, wurden nicht gezählt. Sie müssen es aktivieren, um loszulegen, indem Sie den folgenden Befehl eingeben:

```text
p!config toggle levels
```

### Zulässige Kanäle hinzufügen

Sie können jetzt bestimmte Kanäle hinzufügen, in denen Benutzer XP erhalten können. Die von Ihnen festgelegten Kanäle sind die einzigen Kanäle auf dem Server, in denen Benutzer XP erhalten können. Sie können mehrere Kanäle mit demselben Befehl hinzufügen \(indem Sie ein Leerzeichen zwischen den Kanälen einfügen\) oder Sie können auch Kanäle nacheinander hinzufügen. Um Kanäle hinzuzufügen, können Sie den folgenden Befehl eingeben:

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set xpChannels <Channel/ChannelID/ChannelMention>
```

{% hint style="info" %}
Sie können den Kanal einstellen, indem Sie den Namen des Kanals schreiben, die Kanal-ID verwenden oder den Kanal einfach erwähnen.  
Wenn Sie einen unvollständigen Kanalnamen eingeben, sucht der Bot nach dem nächstgelegenen.
{% endhint %}

{% hint style="success" %}
####  Und Das ist Alles!

Wenn Sie nur das sehr grundlegende Leveling-Setup wünschen, sind Sie jetzt fertig! Wenn Sie mehr in die Tiefe gehen und mehr über die viele weitere Funktionen erfahren möchten, die Sie verwenden können, fahren Sie fort!  
  
_**ALLE SCHRITTE ÜBER DIESEN PUNKT HINAUS SIND OPTIONAL**_
{% endhint %}

### Nicht Zugelassene XP-Rollen hinzufügen

Sie können jetzt bestimmte Rollen so einstellen, dass sie keinen XP erhalten, unabhängig davon, ob sich der Benutzer im entsprechenden Leveling-Kanal befindet oder nicht. Es ist auch nicht wichtig, ob der Benutzer eine andere Rolle über oder unter der Rolle hat, die Sie festgelegt haben um keine XP zu erhalten.   
Diese Funktion ist sehr nützlich, wenn Sie nicht möchten, dass Ihre Mitarbeiter oder Moderatoren XP erhalten, oder um sicherzustellen, dass stummgeschaltete Benutzer keinen XP erhalten usw. Um eine Rolle hinzuzufügen, können Sie den folgenden Befehl eingeben:

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set noXpRoles <Role/RoleID/RoleMention>
```

{% hint style="info" %}
Sie können die Rolle festlegen, indem Sie den Namen der Rolle schreiben, die Rollen-ID verwenden oder einfach die Rolle erwähnen.  
Wenn Sie einen unvollständigen Rollennamen schreiben, sucht der Bot nach dem nächstgelegenen. Dies ist nützlich, wenn Sie System-Emojis als Teil Ihres Rollennamens haben.
{% endhint %}

### Hinzufügen der Top-XP-Rolle

Sie können einen Benutzer auch dafür belohnen, dass er im Server am meisten XP hat, indem Sie dem Bot eine Top-XP-Rolle zuweisen. Diese Rolle wird um 00:00 UTC vergeben und wird immer nur an eine Person auf dem Server vergeben. Wenn ein Benutzer zuvor die Top-XP-Rolle hatte, wird sie ihm entzogen.   
Diese Funktion ist eine schnelle und einfache Möglichkeit, Benutzern ein langfristiges Ziel zu geben, auf das sie hinarbeiten können. Es hilft auch, wenn die Top-XP-Rolle auf der Serverliste recht weit oben steht und eine auffällige Farbe bekommt. Um die Top-XP-Rolle festzulegen, können Sie den folgenden Befehl eingeben:

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set topXpRole <Role/RoleID/RoleMention>
```

{% hint style="warning" %}
Es wird **dringend** empfohlen, auch die Top-XP-Rolle als eine Nicht Zugelassene XP-Rolle festzulegen. Wenn Sie dies nicht tun, kann dies dazu führen, dass immer nur eine Person die Top-XP-Rolle erhält, da sie während ihres Tages an der Spitze weiterhin XP erhalten kann.  
  
Dadurch das Sie sie einen Tag lang keinen XP sammeln lassen, haben andere Benutzer Zeit, aufzuholen.
{% endhint %}

### Anpassen der Level-Up-Nachricht

Wenn Sie feststellen, dass die aktuelle Level-Up-Nachricht nicht zu Ihrem Serverstil passt oder Sie sie einfach ein wenig aufpeppen möchten, können Sie sie vollständig anpassen! Wir unterstützen derzeit leider nur Rohtextnachrichten. \(keine Einbettungen\) Um die Level-Up-Nachricht einzustellen, können Sie den folgenden Befehl eingeben:

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set xpMessage <Message>
```

Es gibt mehrere **Tags**, die Sie in Ihre Level-Up-Nachricht einfügen können. Diese Parameter werden beim Senden der Level-Up-Nachricht durch die entsprechende Information ersetzt.  
  
_You must include the {} brackets in your message for the tags to show up!_

| Information | Tag |
| :--- | :--- |
| Benutzter Erwähnung \(@User\) | {user} |
| Benutzter Tag \(User\#1234\) | {user.tag} |
| Benutzter Name \(User\) | {user.username\) |
| Benutzter Discriminator \(1234\) | {user.discriminator} |
| Benutzter ID \(99787644430475264\) | {user.id} |
| Server Name \(My Cool Server\) | {guild.name} |
| Server ID \(493351982887862283\) | {guild.id} |
| Level Erreicht \(5\) | {level} |

### Wohin die Level-Up-Nachricht gesendet werden soll

Standardmäßig sendet Pepe Manager die Level-Up-Nachricht einfach in dem gleichen Kanal, in dem der Benutzer, der zuletzt gesprochen hat, aber dies kann manchmal aufdringlich sein und die normale Konversation im Kanal stören. Aber keine Sorge, Sie können festlegen, wohin Pepe Manager die Level-Up-Nachricht sendet. Um dies einzurichten, geben Sie einfach den folgenden Befehl ein:

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set xpResponseType <Type>
```

Es gibt mehrere Antworttypen, von denen Sie einen auswählen können. Sie können jeweils nur eine auswählen, und die möglicherweise zuvor eingerichtete Level-Up-Nachricht wird auf jeden Antworttyp übertragen.

| Wohin wird es gesendet? | Antworttyp |
| :--- | :--- |
| Im selben Kanal wie der Benutzer | channel |
| In den Direktnachrichten des Benutzers | dm |
| Immer in einem bestimmten Kanal | \#Channel |
| Nirgends; alle Nachrichten sind aus | off |

### Hinzufügen von Rollenbelohnungen

Sie können Rollen einrichten, die Benutzern zugewiesen werden, wenn sie ein bestimmtes Level erreichen. Dies kann verwendet werden, um einfach das Levels des Benuzters mit einer Rolle anzugeben, Benutzern spezielle Farben zuzuweisen, wenn sie höhere Levels erreichen, Berechtigungen zu vergeben, die durch Aktivität verdient werden können, und vieles mehr.   
Mit der kostenlosen Version von Pepe Manager können Sie bis zu 2 Rollen auf demselben Level vergeben, insgesamt gibt es jedoch _keine_ Begrenzung für die Anzahl der Rollen, die Sie einrichten können. Das [Premium](../information/patreon-perks.md)-limit beträgt 10 Rollen für das gleiche Level.

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set xpRoles <Level> <Role/RoleID/RoleMention>
```

{% hint style="info" %}
Bitte beachten Sie; wenn Ihre Rolle mehrere Wörter enthält, z. B. die Rolle **Cool Person**, müssen Sie entweder die Rollen-ID oder Erwähnung verwenden oder nur das Wort **Cool** schreiben.

Der Bot sieht die Wörter **Cool** und **Person** als separate Rollen.
{% endhint %}

### Levels automatisch Zurücksetzen

Das automatische Zurücksetzen von Levels kann sehr nützlich sein, um Ihren Server sauber und organisiert zu halten und diejenigen, die Sie verbannen, noch mehr zu bestrafen! Wenn die von Ihnen festgelegte Bedingung erfüllt ist, wird Pepe Manager automatisch die Daten des betroffenen Benutzers \(falls vorhanden\) ohne Fragen löschen. **Einen Benutzer vom Server zu treten hat jedoch den gleichen Effekt wie das Verlassen, also sei bitte vorsichtig!**

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set autoResetLevels <Type>
```

Es gibt mehrere Antworttypen, von denen Sie einen auswählen können. Sie können jeweils nur eine auswählen.

| Was löst den Reset aus? | Antworttyp |
| :--- | :--- |
| Nichts | none |
| Wenn der Benutzer den Server aus irgendeinem Grund verlässt | leave |
| Wenn der Benutzer aus irgendeinem Grund verbannt wird | ban |
| Wenn der Benutzer den Server verlässt oder wenn der Benutzer verbannt wird | both |

### Rollenstapelung umschalten

Nachdem Sie nun einige Rollenbelohnungen eingerichtet haben, können Sie auswählen, ob der Bot die Rollen stapeln soll oder nicht. Stapeln bedeutet, dass jede zusätzliche Rollenbelohnung einfach zu den bereits vorhandenen Rollen des Benutzers hinzugefügt wird. Nicht-Staplen bedeutet, dass alle vorherigen Rollenbelohnungen entfernt werden, wenn der Benutzer eine neue Rolle erhält. Dies betrifft nicht Rollen, die nicht ausdrücklich als Belohnungen gekennzeichnet sind.  
Standardmäßig ist das Stapeln **aktiviert**.

```text
p!config toggle stackXpRoles
```

### Letzte Worte

Es ist wirklich einfach, ein Aktivitäts-Tracking-System einzurichten, aber da Sie immer mehr Funktionen hinzufügen und Ihre Benutzer für die Loyalität und Aktivität belohnen möchten, wird es immer komplexer. Wenn Bots neu für Sie sind, haben Sie keine Angst vor all den komplizierten Befehlen und Befehlsstrukturen, neuen Wörtern, die Bots verwenden, um zu beschreiben, was sie tun usw.

Wenn Sie weitere Hilfe zu Pepe Manager benötigen, lesen Sie den Rest dieser Dokumentation oder treten Sie unserem Support-Server bei, um mit einem echten Menschen zu sprechen!

