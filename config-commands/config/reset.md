# Reset

### Description

{% hint style="warning" %}
This is a **method** or **sub-command** of the [Config ](./)command. It is not its own command.
{% endhint %}

This method of the [config ](./)command can be used to reset [toggle ](toggle.md)keys back to their default state.

The reset method **will not** work on set keys, please refer to the delete method!

### Command Structure

Where **&lt; &gt;** is a required parameter

```text
p!config reset <Key>
```

| Key | Description | State When Reset |
| :--- | :--- | :--- |
| counts | Controls if the bot counts member joins & leaves | ❌ \(Off\) |
| emojiList | Controls if the emoji list feature is on or not | ❌ \(Off\) |
| levels | Controls if the leveling feature is on or not | ❌ \(Off\) |
| milestones | Controls if the milestones feature is on or not | ❌ \(Off\) |
| stackXpRoles | Controls if [role rewards](https://docs.pepemanager.com/guides/setting-up-server-xp-leveling#toggling-role-stacking) are stacked or not | ✅ \(Stackable\) |

### **Permission**

* `Manage Server`**\(User\)**
* N/A **\(Bot\)**

### Aliases

* N/A



