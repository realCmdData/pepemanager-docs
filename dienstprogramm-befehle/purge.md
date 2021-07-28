# Reinigen

### Beschreibung

Dieser Befehl kann verwendet werden, um eine große Anzahl von Nachrichten aus einem Channel zu löschen. Dies kann nützlich sein, um nach einem Bot-Angriff aufzuräumen oder um einen Benutzer zu bestrafen, indem alle seine Nachrichten entfernt werden. Der Befehl kann nur bis zu 100 Nachrichten auf einmal bereinigen, wobei nur gültige Nachrichten berücksichtigt werden, die von den Befehls-Tags erfasst werden.

### Befehlstruktur

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert  
Wobei **--Channel** ein Befehls-Tag impliziert  
Wobei **--Benutzer** ein Befehls-Tag einschließt  
Wobei **--Bots** ein Befehls-Tag einschließt

```text
p!purge <Amount> [--Channel] [--User] [--Bots]
```

Die Befehls-Tags müssen als Zusatz zum Befehl verwendet werden:

Der Tag **--Channel** legt fest, in welchem Kanal die Bereinigung stattfinden soll \(Standard ist der Kanal, in dem Sie den Befehl verwenden\)  
Der Tag **--User** legt fest, welche Nachrichten eines Benutzers bereinigt werden sollen. Alle anderen Nachrichten werden in Ruhe gelassen.  
Der Tag **--Bot** legt fest, dass die Bereinigung nur für Nachrichten gelten soll, die von Bots gesendet wurden.

```text
[--Channel] = --Channel [#Channel]
[--User] = --User [@User]
[--Bots] = --Bots
```

### **Berechtigungen**

* `Verwalten von Nachrichten`**\(Benutzer\)**
* `Verwalten von Nachrichten`**\(Bot\)**

### Aliase

* `purge`
* `prune`
* `clear`
* `clean`

