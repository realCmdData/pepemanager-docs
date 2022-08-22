# Bot Permissions

Pepe Manager requires some permissions if you invite it using the default [invite link](https://pepemanager.com/invite). On this page, we will explain why Pepe Manager needs these permissions to function.

{% hint style="danger" %}
Never give any bot **Administrator** permissions, if the bot somehow gets under the control of someone else it could completely destroy your server within moments.
{% endhint %}

| Permission                  | Why Pepe Manager Needs it                                                                                                                                                                                                     |
| --------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Create commands in a server | To create and manage the slash commands you will need to interact with the bot. As of the 22nd of August, Pepe Manager no longer supports prefix commands.                                                                    |
| Manage Emojis               | To Create, Delete and Rename emojis on your server, using the [Createemoji](../emoji-commands/createemoji.md), [Deleteemoji ](../emoji-commands/deleteemoji.md)and [Renameemoji ](../emoji-commands/rename-emoji.md)commands. |
| Read Messages               | To see when a command has been triggered and be able to react to it                                                                                                                                                           |
| Send Messages               | To reply to commands and send an output message                                                                                                                                                                               |
| Manage Messages             | Used for the [Purge ](../utility-commands/purge.md)command and also to delete[ image command messages](../image-commands/banned.md) if the author requests it.                                                                |
| Embed Links                 | Used to create embedded messages, which is how the bot replies to the vast majority of utility commands.                                                                                                                      |
| Attach Files                | Used to send the result of image commands.                                                                                                                                                                                    |
| Read Message History        | Used for the [Purge ](../utility-commands/purge.md)command and also to be able to see when a command has been triggered.                                                                                                      |
| Use External Emojis         | Used to react to confirmation messages with the Pepe Yes Sign and Pepe No Sign emojis                                                                                                                                         |
