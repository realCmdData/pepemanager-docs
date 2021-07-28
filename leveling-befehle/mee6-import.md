# MEE6 Importieren

### Beschreibung

Dieser Befehl kann verwendet werden, um eine bestehende MEE6-Leveling-Datenbank zu importieren, die möglicherweise für Ihren Server existiert. Damit dies funktioniert, muss der MEE6-Bot noch auf Ihrem Server sein und das Leveling-Plugin im MEE6-Dashboard muss noch aktiviert sein.

Standardmäßig werden nur Benutzer bis zur Stufe 5 importiert, um API-Anfragen zu sparen. Wenn Sie jedoch einen viel kleineren Server betreiben, können Sie den optionalen Befehls-Tag verwenden, um diesen Schwellenwert auf Stufe 3 zu senken. Alle Benutzer unterhalb dieser Stufe werden einfach nicht importiert.

Der Befehl importiert nur XP-Zahlen, konvertiert das XP jedoch in die entsprechenden MEE6-Äquivalenzstufen unter Verwendung des MEE6-eigenen Level-Algorithmus. Nach der Konvertierung folgt der Stufenverlauf dem Pepe Manager-eigenen Stufenalgorithmus.

Dieser Befehl hat eine strenge Abklingzeitbegrenzung, um zu verhindern, dass unser Bot von der MEE6-API eine Ratenbeschränkung erhält. Bitte verwenden Sie diesen Befehl nur sparsam.

Sie können die Datenbank auch von einem anderen Server importieren, wenn Sie der Eigentümer sowohl des alten \(Zu importieren von\) als auch des neuen \(Zu importieren in\) Servers sind.

### Befehlstruktur

Wobei **\[ \]** einen optionalen Parameter impliziert  
Wobei **--Until** ein Befehls-Tag impliziert

```text
p!mee6import [ServerID] [--Until]
```

Die Befehls-Tags müssen als Zusatz zum Befehl verwendet werden:

```text
[--Until] = --Until [MEE6 Level]
```

### **Berechtigungen**

* `Server-Eigentümer`**\(Benuzter\)**
* N/A **\(Bot\)**

### Aliase

* `mee6_import`
* `meesix_import`

