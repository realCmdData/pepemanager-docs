---
description: 'Ändere, wer wo wie viel XP erhält!'
---

# Einrichten von XP-Multiplikatoren

### Warum sollten Sie das brauchen?

Mit Pepe Manager können Sie verschiedene XP-Multiplikatoren steuern und sie auf verschiedene Benutzer in verschiedenen Situationen anwenden lassen, um verschiedene Dinge zu belohnen! Ein sehr häufiger Anwendungsfall ist die Belohnung von Boostern mit einem höheren XP-Multiplikator! Sie können auch Ihren gesamten Server-Multiplikator ändern, wenn Sie der Meinung sind, dass die Leute für Ihren Geschmack etwas zu schnell aufsteigen, oder Sie können auch mehr XP in Kanälen geben, in denen die Leute möglicherweise nicht oft sprechen!

### Videoanleitung

Wir haben derzeit noch kein Video-Tutorial für diese Anleitung, schauen Sie später noch einmal vorbei!

## Anleitung

### Stellen Sie sicher, dass Sie die Leveling eingerichtet haben

Bevor Sie dieser Anleitung folgen, stellen Sie bitte sicher, dass Sie das Leveling in Ihrem Server bereits richtig eingerichtet haben. Wenn Sie dabei eine Anleitung benötigen, folgen Sie bitte unserer Anleitung hier:

{% page-ref page="setting-up-server-xp-leveling.md" %}

### Multiplikatoren verstehen

Multiplikatoren mögen gewöhnungsbedürftig sein, aber keine Sorge! Dafür ist diese Anleitung da! Multiplikatoren nehmen im Wesentlichen die Menge an XP, die ein Benutzer normalerweise für eine gültige Nachricht erhalten würde, und multiplizieren sie mit dem Betrag, auf den der Multiplikator eingestellt ist. Wenn ein Benutzer beispielsweise `34` XP für eine Nachricht erhält, der Server jedoch einen globalen Multiplikator von `x1,5` hat, erhält er tatsächlich `51` XP.  
  
Multiplikatoren können jedoch auch unter 1 gesetzt werden, was bedeutet, dass ein Multiplikator von `x0,5` gültig ist, aber das bedeutet _nicht_ einen XP-Gewinn von 50%, sondern einen XP-Verlust von 50%. **Jeder Multiplikator, der über 1 liegt, gibt mehr XP, und jeder Multiplikator, der unter 1 liegt, nimmt XP weg.**

{% hint style="info" %}
Wenn Sie es vorziehen, in Prozenten zu denken; ein Multiplikator von `x1,5` entspricht einem XP-Gewinn von 150% und ein Multiplikator von `x3,4` entspricht einem XP-Gewinn von 340%.
{% endhint %}

### Hierarchie verstehen

Wenn mehr als ein Multiplikator aktiv ist, wird eine Hierarchie erstellt, um zu entscheiden, welcher Multiplikator unter welchen Umständen verwendet wird. _Die Rollenmultiplikatorhierarchie ist etwas anders und wird in_ [_diesem_](https://docs.pepemanager.com/v/deutsch/anleitung/setting-up-xp-multipliers#aendern-der-rollenmultiplikatorhierarchie) _Abschnitt erläutert._

Nehmen wir an, wir haben einen globalen Multiplikator von `x1,1`, einen Kanalmultiplikator von `x1,5` in \#Kanal-A, einen Kanalmultiplikator von `x0,75` in \#Kanal-B und einen weiteren \#Kanal-C ohne Multiplikator:

| Multiplikator | Anwendung |
| :--- | :--- |
| x1.1 | Global |
| x1.5 | \#Channel-A |
| x0.75 | \#Channel-B |
| None | \#Channel-C |

Auf dieser Grundlage möchten wir nun wissen, welcher Multiplikator in jedem Kanal verwendet wird.  
• Wenn wir in \#Kanal-A sprechen, wird der Multiplikator von \#Kanal-A verwendet, da es der höchste derzeit gültige ist.  
• Wenn wir in \#Channel-B sprechen, wird der globale Multiplikator verwendet, da der Kanalmultiplikator niedriger ist als der globale.  
• Wenn wir in \#Channel-C sprechen, wird der globale Multiplikator verwendet, da überhaupt kein Kanalmultiplikator festgelegt ist.

{% hint style="success" %}
Gegebenenfalls wird immer der höchste Multiplikator verwendet!
{% endhint %}

### Globale Multiplikatoren einstellen

Globale Multiplikatoren gelten, wie der Name schon sagt, für den gesamten Server, unabhängig von Rolle, Kanal, Berechtigungen usw. Sie können nützlich sein, wenn Sie den gesamten XP-Gewinn auf Ihrem Server regulieren möchten, zum Beispiel wenn Sie feststellen, dass Ihre Mitglieder XP etwas zu schnellgewinnen, kann die Einführung eines globalen Multiplikators, der kleiner als 1 ist, die Menge der global gewonnenen XP verringern. Um einen globalen Multiplikator hinzuzufügen, können Sie den folgenden Befehl eingeben:

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set xpMultiplier global <Multiplier>
```

{% hint style="info" %}
Mit globalen Multiplikatoren können Sie die Leveling-Kurve an anderer beliebte Bots anpassen!  
_\*Vorausgesetzt sind Standardmäßige_ _XP-Optionen & Multiplikatoren_

**AmariBot •** x0,09  
**Atlas •** x0,22   
**Arcane•** x0,87   
**MEE6 •** x0,65
{% endhint %}

### Kanalmultiplikatoren einstellen

Mit Kanalmultiplikatoren können Sie Multiplikatoren pro Kanal festlegen, aber nicht nur das, Sie können auch mehrere Kanäle auf denselben Multiplikator einstellen oder unterschiedliche Multiplikatoren für mehrere verschiedene Kanäle einstellen! Um einen Kanalmultiplikator hinzuzufügen, können Sie den folgenden Befehl eingeben:

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set xpMultiplier channel <Multiplier> <Channel/ChannelID/ChannelMention>
```

### Rollenmultiplikatoren festlegen

Rollenmultiplikatoren funktionieren ähnlich wie Kanalmultiplikatoren. Sie können demselben Multiplikator mehrere verschiedene Rollen zuweisen oder verschiedene Multiplikatoren für verschiedene Rollen erstellen! Um einen Rollenmultiplikator hinzuzufügen, können Sie den folgenden Befehl eingeben:

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert

```text
p!config set xpMultiplier role <Multiplier> <Role/RoleID/RoleMention>
```

### Ändern der Rollenmultiplikatorhierarchie

Wenn Sie nicht gelesen haben, wie die reguläre Multiplikatorhierarchie funktioniert, lesen Sie bitte zuerst diesen [Abschnitt](https://docs.pepemanager.com/v/deutsch/anleitung/setting-up-xp-multipliers#hierarchie-verstehen).

Die Rollenhierarchie wird **standardmäßig** genauso verwaltet wie alle anderen Multiplikatoren; der höchste anwendbare Multiplikator wird unabhängig von der Rollenhierarchie verwendet. Sie können jedoch die Priorisierung des verwendeten Multiplikators ändern, indem Sie ihn in der Konfiguration umschalten.   
  
Wenn Sie dies tun, wird die höchste Rolle eines Benutzers verwendet, dem auch ein Multiplikator zugeordnet ist, auch wenn eine Rolle mit niedrigerem Rang einen höheren Multiplikator hat. Um die Priorisierung der Rollenhierarchie umzuschalten, können Sie den folgenden Befehl eingeben:

```text
p!config toggle prioritiseMultiplierRoleHierarchy
```



