# Check

### Description

{% hint style="warning" %}
This is a **method** or **sub-command** of the [Config ](./)command. It is not its own command.
{% endhint %}

This method of the [config ](./)command can be used to check if you have inputted all of your configuration keys correctly. The command will reply with an embed containing the key name and the value it is set to.

If a key is not set it will show a 'No Sign' emoji.  
If a **set** key is correctly configured, it will show the value it has been set to.  
Some **set** keys are configured to a default value, which will also been shown on the check command.  
If a **toggle** key is set to true, it will show a 'Yes Sign' emoji, and if set to false it will show a 'No Sign' emoji.

### Command Structure

```text
p!config check
```

Below is a table containing all configuration keys that are shown in the check method, alongside all of the default values.

| Key | Default Check Value |
| :--- | :--- |
| Milestones Channel | ❌ \(Not Set\) |
| Milestone Interval | ✅ \(100\) |
| Prefix | ✅ \(p!\) |
| Member Count | ✅ \(On\) |
| Auto Role | ❌ \(Not Set\) |
| Auto Role Timeout | ❌ \(Not Set\) |
| Emoji List | ❌ \(Not Set\) |
| Blacklisted Channels | ❌ \(Not Set\) |
| XP Channels | ❌ \(Not Set\) |
| XP Roles | ❌ \(Not Set\) |
| Stack XP Roles | ✅ \(True\) |
| Top XP Role | ❌ \(Not Set\) |
| No XP Roles | ❌ \(Not Set\) |
| Auto Publish Channels | ❌ \(Not Set\) |
| Role Mention Cooldown | ✅ \(0ms\) |
| Mention Cooldown Roles | ❌ \(Not Set\) |
| XP Response Type | ✅ \(Same Channel\) |
| XP Message | ✅ \({user} has reached level **{level}**\) |
| Milestone Message | ✅ \(**{milestone} Members**  Congratulations to {user}, you were the {milestone}th person to join!\) |

### **Permission**

* `Manage Server`**\(User\)**
* N/A **\(Bot\)**

### Aliases

* N/A



