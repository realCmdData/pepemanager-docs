# Troubleshoot

### Description

{% hint style="warning" %}
This is a **method** or **sub-command** of the [Config ](./)command. It is not its own command.
{% endhint %}

This method of the [config ](./)command can be used to check if features of Lurkr have been correctly configured either using the dashboard or some of the other methods of the config command.&#x20;

The troubleshoot embed can tell you whether everything is configured correctly, if a features is turned off (and therefore won't be checked) or if there is a problem, what is causing it, letting you deduce how you can fix it!

### Command Structure

```
/config troubleshoot
```

<figure><img src="https://i.imgur.com/aP7p1lT.png" alt=""><figcaption></figcaption></figure>

### Possible Checks

Below is a list of checks that the troubleshoot command can perform and will alert you of.

This table can also show you in more detail what is meant by each error and how you can generally fix them!

| Error                          |                                                       Meaning                                                       |                                                                                                                                                                                Fix |
| ------------------------------ | :-----------------------------------------------------------------------------------------------------------------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| Channel not found              |                                    The channel doesn't exist or never did exist.                                    |                                                Set a channel that does exist to Lurkr. Use channel ID's to tell exactly which channel should be used if there are duplicate names. |
| Invalid channel types          |          The channel can't be used in this context. For example, voice channels can't be leveling channels.         |                                                                                                Set a channel that Lurkr does support, like normal text channels or forum channels. |
| Missing permissions on channel |                               Lurkr doesn't have necessary permission for the channel                               |                                                                                        Give Lurkr either server-wide or in the channel the [needed permissions](broken-reference). |
| Role not found                 |                                      The role doesn't exist or never did exist.                                     |                                                         Set a role that does exist to Lurkr. Use role ID's to tell exactly which role should be used if there are duplicate names. |
| Role not editable              |                      The role cannot be edited by Lurkr, and therefore can't be given to users.                     | This cannot be fixed as it happens with integration [managed roles](https://support.discord.com/hc/en-us/articles/360045093012-Server-Integrations-Page). Choose a different role. |
| Role hierarchy incorrect       | Lurkr's top most role is below one or more of the roles you want to set, not allowing Lurkr to control those roles. | Either move the roles higher than Lurkr's highest role or the opposite. [Learn about role hierarchy](https://support.discord.com/hc/en-us/articles/214836687-Role-Management-101). |



### **Permission**

* `Manage Server`**(User)**
* N/A **(Bot)**

### Aliases

* N/A

