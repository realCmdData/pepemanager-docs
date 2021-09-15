# Toggle

### Description

{% hint style="warning" %}
This is a **method** or **sub-command** of the [Config ](./)command. It is not its own command.
{% endhint %}

This method of the [config ](./)command can be used to toggle a set of keys that are listed below. These keys are booleans, meaning that they can only be turned either on or off, or set from one value to another.  
Toggle keys are mostly used to turn specific features of Pepe Manager on or off.

### Command Structure

Where **&lt; &gt;** is a required parameter

```text
p!config toggle <Key>
```

| Key | Description | Default State |
| :--- | :--- | :--- |
| counts | Controls if the bot counts member joins & leaves | ✅ \(On\) |
| emojiList | Controls if the emoji list feature is on or not | ❌ \(Off\) |
| levels | Controls if the leveling feature is on or not | ❌ \(Off\) |
| milestones | Controls if the milestones feature is on or not | ❌ \(Off\) |
| prioritiseMultiplierRoleHierarchy | Controls if [role prioritisation](https://docs.pepemanager.com/guides/setting-up-xp-multipliers#changing-role-multiplier-hierarchy) is on or not | ❌ \(Multiplier Value\) |
| stackXpRoles | Controls if [role rewards](https://docs.pepemanager.com/guides/setting-up-server-xp-leveling#toggling-role-stacking) are stacked or not | ✅ \(Stackable\) |
| xpInThreads | Controls if [leveling XP](../../guides/setting-up-server-xp-leveling.md) is gained in threads | ❌ \(Off\) |

### **Permission**

* `Manage Server`**\(User\)**
* N/A **\(Bot\)**

### Aliases

* N/A



