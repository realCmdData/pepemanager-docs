# Purge

### Description

This command can be used to purge or clean a large number of messages from a channel. This can be useful to clean up after a bot raid or to punish a user by removing all of their messages.

The command can only purge up to 100 messages at a time, which only accounts for valid messages picked up by your command tags.

### Command Structure

Where **&lt; &gt;** implies a required parameter  
Where **--Channel** implies a command tag   
Where **--User** implies a command tag  
Where **--Bots** implies a command tag

```text
p!purge <Amount> [--Channel] [--User] [--Bots]
```

The command tags need to be used as an addition to the command:

The **--Channel** tag defines in which channel the purge should take place in \(Default is the channel you use the command in\)  
The **--User** tag defines which user's messages should be purged. All other messages will be left alone.  
The **--Bot** tag defines that the purge should only apply to messages sent by bots.

```text
[--Channel] = --Channel [#Channel]
[--User] = --User [@User]
[--Bots = --Bots
```

### **Permission**

* `Manage Messages` **\(User\)**
* `Manage Messages`**\(Bot\)**

### Aliases

* `purge`
* `prune`
* `clear`
* `clean`

