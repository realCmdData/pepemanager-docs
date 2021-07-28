# Delete

### Description

{% hint style="warning" %}
This is a **method** or **sub-command** of the [Config ](./)command. It is not its own command.
{% endhint %}

This method of the [config ](./)command can be used to delete the keys that are listed below. Once a key is deleted there is no way to retrieve it, and must be set manually again.

The delete method **will not** work on toggle keys, please refer to the [reset ](reset.md)method!

### Command Structure

Where **&lt; &gt;** is a required parameter

```text
p!config delete <Key>
```

| Key | Description |
| :--- | :--- |
| autoPublishChannels | [Announcement channels](https://support.discord.com/hc/en-us/articles/360032008192-Announcement-Channels-) you want to automatically publish  |
| autoResetLevels | Automatically resets user levels if the conditions you set are met |
| autoRole | Roles you want to automatically assign to new members |
| autoRoleTimeout | Length of time between a user joining and getting a role |
| blacklistedChannels | Channels in which Pepe Manager commands don't work |
| emojiListChannel | The channel for the automated emoji list |
| mentionCooldown | Length of time between role mentions |
| mentionCooldownRoles | Pingable roles you want to have a ping cooldown on |
| milestonesChannel | The channel for all milestone announcements |
| milestonesInterval | The number of members between milestones |
| milestonesMessage | The message sent out when a milestone is reached |
| milestonesRole | The role\(s\) that is given to the person who joins as the milestone is reached |
| noXpRoles | Roles you do not want to gain XP in the whole server |
| prefix | The server-prefix you want the bot to use \(Default is p!\) |
| topXpRole | The role you want to give to the user leading the leaderboard that day |
| xpBlacklistedChannels | Channels you **do not** want XP to be gained in. All other channel will be able to gain XP |
| xpMessage | The message sent out when someone levels-up |
| xpMultiplier | Set different multipliers for variable XP gain |
| xpResponseType | The destination of a level-up message |
| xpRoles | Role rewards you want to give out at a specific level |
| xpWhitelistedChannels | Channels you **want** XP to be gained in. All other channel will not be able to gain XP |

### **Permission**

* `Manage Server`**\(User\)**
* N/A **\(Bot\)**

### Aliases

* `del`
* `remove`
* `rm`



