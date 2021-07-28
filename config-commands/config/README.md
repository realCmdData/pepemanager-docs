# Config

### Description

{% hint style="warning" %}
**We know this command is complex**. Please read all of the documentation so you fully understand how it works. If you still need help with the command, you are more than welcome to ask in our \#bot-support channel.
{% endhint %}

This command can be used to configure how Pepe Manager behaves in your server. Most, if not all of the settings you can change about Pepe Manager can be done through the configuration command.

Each **sub-command** or **method** contains its own **keys**. Keys are the individual configuration options you can change, and the **method** or **sub-command** is the way in which you can interact with these keys.

### Command Structure

Where **&lt; &gt;** implies a required parameter  
Where **\[ \]** implies an optional parameter

```text
p!config <Method> [Arguments]
```

| Methods | Description |
| :--- | :--- |
| check | Displays an embed with all of your configuration options and how they have been set |
| delete | Completely removes an entry to a **set** key |
| deleteall | Completely removes all configuration options you have set |
| reset | Resets an entry to a **toggle** key back to its original state |
| set | Sets a key to a specified value |
| toggle | Toggles a key to true or false |

### **Permission**

* `Manage Server`**\(User\)**
* N/A **\(Bot\)**

### Aliases

* `config`
* `cfg`



