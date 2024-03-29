# Set

### Description

{% hint style="warning" %}
This is a **method** or **sub-command** of the [Config ](./)command. It is not its own command.
{% endhint %}

This method of the [config ](./)command can be used to set the options that are listed below. You can delete an already set option by using the **delete** method.

The set method **will not** work on toggle options, please refer to the [toggle](broken-reference) method!

### Command Structure

```
/config set <option:> [values:]
```

| Option                                  |                                                                                   Description |
| --------------------------------------- | --------------------------------------------------------------------------------------------: |
| On Join Roles                           |                             The roles you want your members to get when they join your server |
| On Join Roles for Badges                |         The roles you want your members with Discord badges to get when they join your server |
| On Join Role Timer                      |                   The time it takes between a member joining your server and getting the role |
| Emoji List Channel                      |                                    The channel you want the bot to list all of your emojis in |
| Default Leveling Card Accent Colour     | The default progress bar colour you want your members to have when they use the /rank command |
| Automatic Level Resets                  |                                              How the bot will treat automatic leveling resets |
| No Leveling Roles                       |                                            The roles you don't want to be able to gain levels |
| No Top Leveling Roles                   |                              The roles you don't want to be able to get the Top Leveling role |
| Daily Top Leveling Role                 |                  The role you want members to get when they are number one on the leaderboard |
| Leaderboard Vanity URL                  |                                   The vanity URL you want to have for your server leaderboard |
| Specific Announcement Levels            |                        The specific levels you want to be announced when someone reaches them |
| Minimum Leveling Announcement Threshold |                            The minimum level you want to be announced when someone reaches it |
| Factor for Leveling Announcements       |                       The factor of levels you want to be announced whe nsomeone reaches them |
| Leveling Channels                       |                                               The channels you want members to gain levels in |
| Ignored Leveling Bot Prefixes           |                                The prefixes of text-bots that should be ignored from leveling |
| Level Up Message                        |                                             The message that gets sent when someone levels up |
| Setup Leveling Multiplier               |                                       The multipliers you want to have in effect for leveling |
| Level Up Message Destination            |                           The place you want levels to be announced when someone reaches them |
| Setup Leveling Role Rewards             |                               The roles you want to give members for reaching a certain level |
| Role Mention Cooldown Time              |                                                        The minimum time between role mentions |
| Role Mention Cooldown Roles             |                                              The roles you want to have on a mention cooldown |
| Milestone Channel                       |                                   The channel you want to send all milestone announcements to |
| Milestone Announcement Interval         |                             The amount of members that need to join before the next milestone |
| Milestone Announcement Message          |                              The message that will be sent when the next milestone is reached |
| Milestone Reward Roles                  |                        The role(s) you want to give to the member who joined on the milestone |
| Auto-Publishing Announcement Channels   |                            The announcement channels you want to be auto-published by the bot |

### **Permission**

* `Manage Server`**(User)**
* N/A **(Bot)**

