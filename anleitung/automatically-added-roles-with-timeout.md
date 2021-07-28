---
description: >-
  Lernen Sie, wie Pepe Manager neuen Benutzerrollen automatisch zuweisen kann,
  ohne das Discord-Verifizierungssystem zu durchbrechen!
---

# Rollen automatisch hinzufügen \(mit Timeout\)

### Warum sollten Sie das brauchen?

Das automatische Hinzufügen von Rollen zu neuen Mitgliedern kann viele nützliche Zwecke erfüllen, von neuen Mitgliedern in Ihrem Chat eine coole Farbe zu geben, Berechtigungsrollen zu vergeben, die bei Bedarf entfernt werden können, oder um Ping-Rollen für Ankündigungen hinzuzufügen.   
Wenn Sie jedoch eine Discord-Verifizierungsebene aktiviert haben, die dazu führt, dass Benutzer, die die erforderliche Verifizierungsebene überschreiten wenn ihnen automatisch eine Rolle hinzugefügt wird, wird dieser Verifizierungsfilter umgangen! Mit Pepe Manager können Sie einen Timer ab dem Zeitpunkt einstellen, an dem ein Benutzer beitritt, bis er die Rolle erhält, damit das Verifizierungssystem nicht umgangen wird!

### Videoanleitung

Wenn Sie langes Lesen abgeneigt sind, haben wir ein Video-Tutorial erstellt, das leicht zu verstehen sein sollte:

**\(NUR AUF ENGLISCH ERHÄLTLICH\)**

{% embed url="https://youtu.be/94NleboBP\_o" %}

## Anleitung

### Bewertung Ihres Verifizierungslevels

Damit diese Anleitung am effektivsten ist, sollten Sie in Ihre Servereinstellungen gehen, zur Registerkarte Moderation gehen und noch einmal überprüfen, welche Verifizierungsstufe Sie ausgewählt haben.

![](https://i.imgur.com/dZ9o0ae.png)

Die Verifizierungsstufe **Mittel** hat eine Zeitüberschreitung von 5 Minuten, während die Einstellungen **Hoch** und **Höchste** eine Zeitüberschreitung von 10 Minuten haben.

### Einstellen Ihrer Autorollen

Sie können jetzt Ihre Autorollen zu Pepe Manager hinzufügen. In der aktuellen Version ist es nicht möglich, verschiedenen Timeouts unterschiedliche Rollen zuzuweisen, sie werden alle gleichzeitig zugewiesen.  
In der kostenlosen Version des Bots können Sie bis zu 5 Autorollen gleichzeitig zuweisen, während Sie in der Premium-Version bis zu 25 Autorollen zuweisen können. [Klicken sie hier um mehr zu erfahren](../information/patreon-perks.md).

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set autoRole <Role/RoleID/RoleMention>
```

{% hint style="warning" %}
Sie können alle Ihre Autorollen mit demselben Befehl festlegen, indem Sie einfach ein Leerzeichen zwischen den einzelnen Rollen einfügen. Dies funktioniert jedoch nur für Rollenerwähnungen und Rollen-IDs, wenn eine oder mehrere der Rollen, die Sie zuweisen möchten, ein Leerzeichen im Namen haben.  
Leerzeichen werden als Trennzeichen behandelt, und wenn Sie den vollständigen Rollennamen mit einem Leerzeichen eingeben, behandelt Pepe Manager sie als 2 separate Rollen.
{% endhint %}

### Einstellen Ihres Timeouts

Sie können jetzt angeben, wie lange der Bot warten soll, bevor er die Rollen zuweist, nachdem ein Benutzer beigetreten ist. Dies ist nicht auf 5 Minuten oder 10 Minuten beschränkt, Sie können das Timeout auf nur 1 Minute oder bis zu 30 Minuten einstellen.

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set autoRoleTimeout <Time>
```

### Letzte Worte

Und das ist es! Sie haben die automatische Rollenzuweisung mit Pepe Manager erfolgreich erstellt!

Wenn Sie weitere Hilfe zu Pepe Manager benötigen, lesen Sie den Rest dieser Dokumentation oder treten Sie unserem Support-Server bei, um mit einem echten Menschen zu sprechen!

