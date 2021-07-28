# Set

### Description

{% hint style="warning" %}
This is a **method** or **sub-command** of the [Config ](./)command. It is not its own command.
{% endhint %}

This method of the [config ](./)command can be used to set the keys that are listed below. The value that you can set keys to varies depending on what key you are trying to set.

### Command Structure

Where **&lt; &gt;** is a required parameter

```text
p!config set <Key> <Value>
```

| Key | Description | Accepted Value |
| :--- | :--- | :--- |
| autoPublishChannels | [Announcement channels](https://support.discord.com/hc/en-us/articles/360032008192-Announcement-Channels-) you want automatically publish  | Channel\(s\) |
| autoResetLevels | Automatically resets user levels if the conditions you set are met | [See Here](https://docs.pepemanager.com/guides/setting-up-server-xp-leveling#automatically-resetting-levels) |
| autoRole | Roles you want to automatically assign to new members | Role\(s\) |
| autoRoleTimeout | Length of time between a user joining and getting a role | Time Interval |
| blacklistedChannels | Channels in which Pepe Manager commands don't work | Channel\(s\) |
| emojiListChannel | The channel for the automated emoji list | Channel |
| mentionCooldown | Length of time between role mentions | Time Interval |
| mentionCooldownRoles | Pingable roles you want to have a ping cooldown on | Role\(s\) |
| milestonesChannel | The channel for all milestone announcements | Channel |
| milestonesInterval | The number of members between milestones | Any Multiple of 5 |
| milestonesMessage | The message sent out when a milestone is reached | Message |
| milestonesRole | The role\(s\) that is given to the person who joins as the milestone is reached | Role\(s\) |
| noXpRoles | Roles you do not want to gain XP in the whole server | Role\(s\) |
| prefix | The server-prefix you want the bot to use \(Default is p!\) | Alphanumeric Values & Symbols |
| topXpRole | The role you want to give to the user leading the leaderboard that day | Role |
| xpBlacklistedChannels | Channels you **do not** want XP to be gained in. All other channel will be able to gain XP | Channel\(s\) |
| xpMessage | The message sent out when someone levels-up | Message |
| xpMultiplier | Set different multipliers for variable XP gain | [See Here](../../guides/setting-up-xp-multipliers.md) |
| xpResponseType | The destination of a level-up message | [See Here](https://docs.pepemanager.com/guides/setting-up-server-xp-leveling#where-to-send-the-level-up-message) |
| xpRoles | Role rewards you want to give out at a specific level | [See Here](https://docs.pepemanager.com/guides/setting-up-server-xp-leveling#adding-role-rewards) |
| xpWhitelistedChannels | Channels you **want** XP to be gained in. All other channel will not be able to gain XP | Channel\(s\) |

### Value Structure

Below is a table outlining what each of the values listed above will accept in detail. 

<table>
  <thead>
    <tr>
      <th style="text-align:left">Accepted Value</th>
      <th style="text-align:left">What it Includes</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Channel(s)</td>
      <td style="text-align:left">
        <p>&#x2022; Channel Mentions (#Channel)</p>
        <p>&#x2022; Channel Names (Channel)</p>
        <p>&#x2022; Channel IDs (841218613380644914)</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Role(s)</td>
      <td style="text-align:left">
        <p>&#x2022; Role Mentions (@Role)</p>
        <p>&#x2022; Role Names (Role)</p>
        <p>&#x2022; Role IDs (493352184377901066)</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Time Interval</td>
      <td style="text-align:left">
        <p>&#x2022; 60 seconds (60s)</p>
        <p>&#x2022; 1 minute (1m)</p>
        <p>&#x2022; 3 hours (3h)</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Message</td>
      <td style="text-align:left">&#x2022; Any Valid Discord Message</td>
    </tr>
    <tr>
      <td style="text-align:left">Any Multiple of 5</td>
      <td style="text-align:left">&#x2022; Any number that is a multiple of 5 (10, 15, 50, 10000, 750)</td>
    </tr>
    <tr>
      <td style="text-align:left">Alphanumeric Values &amp; Symbols</td>
      <td style="text-align:left">&#x2022; Any character that is either a number (1, 2, 3) or a letter (a,
        b, c) or a common symbol (!, $, %)</td>
    </tr>
  </tbody>
</table>

### **Permission**

* `Manage Server`**\(User\)**
* N/A **\(Bot\)**

### Aliases

* N/A



