# Growth Change

### Description

This command can be used to visualize the **change** in user growth on your server over time. You can change the number of days the graph displays with the days command tag.

Note that the bot can only display user growth while it is in your server. As long as it isn't in your server it cannot track users in any way. Please also note that by toggling the configuration option `counts` it will prevent the bot from tracking users even while it is still in the server.  
  
This command is different from the `graph` command because it shows the change in user growth, not the total overall growth. In this case, the graph can be negative if you lose more users than you gain.

### Command Structure

Where **\[ \]** implies an optional parameter  
Where **--Days** implies a command tag

```text
p!growthchange [--Days]
```

The command tag needs to be used as an addition to the command:

```text
[--Days] = --Days [Number]
```

### **Permission**

* N/A **\(User\)**
* `Embed Links`**\(Bot\)**

### Aliases

* `growth_change`
* `growth_delta`

