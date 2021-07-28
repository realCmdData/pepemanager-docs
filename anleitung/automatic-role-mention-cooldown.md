---
description: >-
  Erfahren Sie, wie Sie automatisch steuern, wer eine bestimmte Rolle erwähnen
  darf!
---

# Automatische Abklingzeit für Rollenerwähnungen

### Warum sollten Sie das brauchen?

Der Hauptanwendungsfall dieser Funktion besteht darin, dass viele Server ihre Moderatorrolle erwähnenswert halten möchten, falls ein Unfall oder eine Katastrophe passiert, um die Moderatoren so schnell wie möglich in Bereitschaft zu halten. Wenn diese Macht jedoch zu vielen Leuten gegeben wird, wird es irgendwann Leute geben, die dies missbrauchen und Moderatoren ständig spammen, auch wenn kein Notfall vorliegt.

### Videoanleitung

Wir haben derzeit noch kein Video-Tutorial für diese Anleitung, schauen Sie später noch einmal vorbei!

## Anleitung

### Einrichten der Rollen

Um zu beginnen, müssen Sie zunächst festlegen, welche Rollen eine Abklingzeit für Erwähnungen haben sollen. Normalerweise ist dies die Moderatorenrolle oder die Administratorrolle, es liegt jedoch ganz bei Ihnen, für welche Rolle\(n\) Sie sich entscheiden. Geben Sie den folgenden Befehl ein, um Ihre Rolle\(n\) festzulegen:

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set mentionCooldownRoles <Role/RoleID/RoleMention>
```

### Einstellen der Abklingzeit

Die Abklingzeit kann zwischen 5 Minuten und 30 Minuten betragen und ist die Zeit zwischen der Deaktivierung der Rollenerwähnungsoption nach einer Erwähnung in einem Kanal und ihrer erneuten Aktivierung. Geben Sie den folgenden Befehl ein, um Ihre Abklingzeit einzustellen:

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set mentionCooldown <Time>
```

### Letzte Worte

Und das ist es! Sie haben mit Pepe Manager erfolgreich automatische Abklingzeiten für Rollenerwähnungen erstellt! 

Wenn Sie weitere Hilfe zu Pepe Manager benötigen, lesen Sie den Rest dieser Dokumentation oder treten Sie unserem Support-Server bei, um mit einem echten Menschen zu sprechen!

