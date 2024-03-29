# Purge

### Description

{% hint style="info" %}
Even though this might be classed as a 'moderation' command, we see it more as a utility command.

We have no intentions of ever adding moderation commands since that's not the purpose of Lurkr.
{% endhint %}

This command can be used to purge or clean a large number of messages from a channel. This can be useful to clean up after a bot raid or to punish a user by removing all of their messages.

The command can only purge up to 100 messages at a time, which only accounts for valid messages picked up by your command tags.

### Command Structure

```
/purge <amount:> [channel:] [user:] [only_bots:] [include_pinned:]
```

<figure><img src="https://i.imgur.com/SJymocg.png" alt=""><figcaption></figcaption></figure>

The command options can be used as an addition to the command:

The `channel:` options defines in which channel the purge should take place in (Default is the channel you use the command in)

The `user:` options defines which user's messages should be purged. All other messages will be left alone.

The `only_bots:` options defines if the purge should only apply to messages sent by Discord bots with the blue BOT badge.

The `include_pinned:` option defines whether or not the purge should include messages that have been pinned in the channel.

### **Permission**

* `Manage Messages` **(User)**
* `Manage Messages`**(Bot)**
