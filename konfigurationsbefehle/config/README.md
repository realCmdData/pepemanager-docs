# Konfiguration

### Beschreibung

{% hint style="warning" %}
**Wir wissen, dass dieser Befehl komplex ist.** Bitte lesen Sie die gesamte Dokumentation, damit Sie die Funktionsweise vollständig verstehen. Wenn Sie noch Hilfe beim Befehl benötigen, können Sie gerne in unserem [\#bot-support](https://discord.gg/2qWnHFkGJ7) Kanal nachfragen.
{% endhint %}

Mit diesem Befehl können Sie konfigurieren, wie sich Pepe Manager auf Ihrem Server verhält. Die meisten, wenn nicht alle Einstellungen, die Sie über Pepe Manager ändern können, können über den Konfigurationsbefehl vorgenommen werden.

Jeder **Unterbefehl** oder jede **Methode** enthält seine eigenen **Schlüssel**. Schlüssel sind die einzelnen Konfigurationsoptionen, die Sie ändern können, und die **Methode** oder der **Unterbefehl** ist die Art und Weise, wie Sie mit diesen Schlüssel interagieren können.

### Befehlstruktur

Wobei **&lt; &gt;** einen erforderlichen Parameter impliziert  
Wobei **\[ \]** einen wahlfreien Parameter impliziert

```text
p!config <Method> [Arguments]
```

| Methoden | Beschreibung |
| :--- | :--- |
| check | Zeigt eine Einbettung mit all Ihren Konfigurationsoptionen und deren Einstellung an |
| delete | Entfernt einen Eintrag zu einem **set** Schlüssel vollständig |
| deleteall | Entfernt vollständig alle Konfigurationsoptionen, die Sie eingestellt haben |
| reset | Setzt ein Eintrag eines **toggle** Schlüssels in den ursprünglichen Zustand zurück |
| set | Setzt einen Schlüssel auf einen bestimmten Wert |
| toggle | Schaltet einen Schlüssel auf wahr oder falsch um |

### **Berechtigungen**

* `Server verwalten` **\(Benutzer\)**
* N/A **\(Bot\)**

### Aliase

* `config`
* `cfg`



