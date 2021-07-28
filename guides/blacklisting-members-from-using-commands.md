---
description: Learn how to restrict Pepe Manager to only certain channels!
---

# Blacklisting Members from using Commands

### Why Would You Need This?

Moderating a server is already harder than it needs to be. And keeping all of the bots confined to one or multiple channels to stop users from using and/or abusing them in general channels is hard as well. The easiest way to keep everything where it's supposed to be is with blacklisting. Only allow Pepe Manager to respond to commands in designated areas.  

### Video Tutorial <a id="video-tutorial"></a>

We currently do not have a video tutorial for this guide just yet, check back later!

## Guide <a id="guide"></a>

### Understanding how the Blacklist works <a id="understanding-how-the-blacklist-works"></a>

Blacklisting a channel using Pepe Manager is quite similar to simply using permissions to restrict who can use commands in what channel, however it is much easier to do.

When a channel is blacklisted, all members who can chat in said channel regularly, will no longer be able to execute Pepe Manager commands. This does not however apply to server Administrators, ie. anyone with the Admin permission.

If you have the Admin permission, you will bypass the blacklist, even if it is working as intended.

### Adding Blacklisted Channels <a id="adding-blacklisted-channels"></a>

To add channels to the blacklist you can execute the command below, including as many channels as you want. You can always add more channels later down the line if you choose to, and you can also delete channels as you see fit.

Where **&lt; &gt;** implies a required parameter

```text
p!config set blacklistedChannels <Channel/ChannelID/ChannelMention>
```

### Removing Blacklisted Channels <a id="removing-blacklisted-channels"></a>

Removing channels from the blacklist is almost as easy as adding them, just in reverse! Of course keep in mind that in order to remove a channel from the blacklist it first needs to be on it. To remove one or multiple channels from the blacklist, execute the following command:

Where **&lt; &gt;** implies a required parameter

```text
p!config delete blacklistedChannels <Channel/ChannelID/ChannelMention>
```

### Final Words <a id="final-words"></a>

And that's it! You've successfully learnt how to add and remove blacklisted channels from Pepe Manager to manage your server more efficiently!

If you need any more assistance with Pepe Manager, check out the rest of this documentation or join our support server to talk to an actual human![  
](https://discord.gg/pepe)

