# Level

### Description

This command can be used to view your current level, how much total XP you have gained, how much XP you need to advance to the next level, and if you are using the image level card, also shows you a progress bar to the next level.

You can also input another user on the server to view their leveling information. The same information will be shown as with your leveling information.

When requesting an image leveling card, the bot will also add a **Text Mode** button. Either the author of the command or the user who was mentioned (If applicable) can press this button to request a more mobile-friendly, text-only version of the same command. This can also be accomplished by including the  **--text** tag when writing the command initially.\
\
When requesting an image leveling card, the bot will also add a **Sync** button. The author of the command can press the button in order to try and synchronize the role rewards with the current level. This could be useful if a new role reward has been added, and the user is already above the level required but doesn't have the role yet.

![An example of an image leveling card](../.gitbook/assets/default.png)

### Command Structure

Where **\[ ]** implies an optional parameter\
Where **--Text** implies a command tag

```
p!level [@User/UserID] [--Text]
```

### **Permission**

* N/A **(User)**
* `Attach Files`**(Bot)**

### Aliases

* `level`
* `lvl`
* `rank`
