# Config

{% hint style="success" %}
**We have a dashboard!**\
Everything you can do with the config command you can now do in our user-friendly web-interface! Simply log-in to our website [https://pepemanager.com/](https://pepemanager.com/) and select the server you want to configure!
{% endhint %}

### Description

{% hint style="warning" %}
**We know this command is complex**. Please read all of the documentation so you fully understand how it works. If you still need help with the command, you are more than welcome to ask in our [#support](https://pepemanager.com/support) channel.
{% endhint %}

This command can be used to configure how Pepe Manager behaves in your server. Most, if not all of the settings you can change about Pepe Manager can be done through the configuration command.

The config command has 6 **methods**, or ways to interact with the command. These are represented as sub-commands. Within each **method** you have a **category** which corresponds to the major feature categories that you can configure in Pepe Manager. Once you've select the method and category, you can then set an option, which is the specific setting you want to configure.

### Command Structure

```
/config <Method> <Category> [option:]
```

| Methods                    | Description                                                                         |
| -------------------------- | ----------------------------------------------------------------------------------- |
| [check](check.md)          | Displays an embed with all of your configuration options and how they have been set |
| [delete](delete.md)        | Completely removes an entry to a **set** option                                     |
| [deleteall](delete-all.md) | Completely removes all configuration options you have configured                    |
| [reset](reset.md)          | Resets an entry of a **toggle** option back to its original state                   |
| [set](set.md)              | Sets an option to a specified value                                                 |
| [toggle](toggle.md)        | Toggles an option to true or false                                                  |

### **Permission**

* `Manage Server`**(User)**
* N/A **(Bot)**

