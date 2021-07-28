# Wachstum Veränderung

### Beschreibung

Dieser Befehl kann verwendet werden, um die **Veränderung** des Benutzerwachstums auf Ihrem Server im Laufe der Zeit zu visualisieren. Sie können die Anzahl der Tage, die das Diagramm anzeigt, mit dem Befehls-Tag days ändern.

Beachten Sie, dass der Bot das Nutzerwachstum nur anzeigen kann, solange er sich auf Ihrem Server befindet. Solange er sich nicht auf Ihrem Server befindet, kann er keine Benutzer verfolgen. Bitte beachten Sie auch, dass das Umschalten der Konfigurationsoption **counts** den Bot daran hindert, Benutzer zu verfolgen, auch wenn er sich noch auf dem Server befindet.  
  
Dieser Befehl unterscheidet sich vom [Diagramm](graph.md)-Befehl, da er die Veränderung des Nutzerwachstums und nicht das Gesamtwachstum anzeigt. In diesem Fall kann das Diagramm negativ sein, wenn Sie mehr Nutzer verlieren als gewinnen.

### Befehlstruktur

Wobei **\[ \]** einen optionalen Parameter impliziert  
Wobei **--Days** ein Befehls-Tag impliziert

```text
p!growthchange [--Days]
```

Das Befehls-Tag muss als Zusatz zum Befehl verwendet werden:

```text
[--Days] = --Days [Number]
```

### **Berechtigungen**

* N/A **\(Benutzer\)**
* `Links einbetten`**\(Bot\)**

### Aliase

* `growth_change`
* `growth_delta`

