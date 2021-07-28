---
description: >-
  Set up a list of all of your server emojis and forget about it as it updates
  itself
---

# Automatically Controlled Emoji-List

### Why Would You Need This?

An essential feature of Discord Emoji Servers is the conveniently created Emoji-Lists. Conventionally they are one channel dedicated to listing all of the emojis that are in one server or in some cases a multitude of servers, so users can easily copy and paste their favourite ones, look for enticing emojis to use, and more.   
Pepe Manager offers exactly this, plus it gives you the freedom to set it up and forget about it as it does all of the work in the background.

### Video Tutorial

If you are averse to long bouts of reading, we have created a video tutorial that should be easy to follow along:  


{% embed url="https://youtube.com/watch?v=CYMIeDcgeek" %}

## Guide

### Setting the Channel

The first thing you want to do is create a channel for your emoji list. This will be the final channel, so set it up in the way you want everyone to see it.

Next, you want to enter the following command:

Where **&lt; &gt;** implies a required parameter

```text
p!config set emojiListChannel <Channel/ChannelID/ChannelMention>
```

{% hint style="info" %}
You can set the channel by writing the name of the channel, using the channel ID or by simply mentioning the channel.  
If you write an incomplete channel name the bot will look for the next closest one.
{% endhint %}

### Enabling the List

Next, you will want to enable the emoji list. By default, even if you have set the emojiListChannel, it is not enabled. To enable it, enter the following command:

```text
p!config toggle emojiList
```

### Update the List

Finally, to get your new emoji list going, you need to manually update the emoji list. This is the only time you need to update it manually, however, you can always update the list manually later down the line:

```text
p!updateemojilist
```

### Final Words

And that's it! You've successfully created an Automatically Controlled Emoji-List with Pepe Manager!

The Emoji-List will automatically update on these events:

* An Emoji is created
* An Emoji is deleted
* An Emoji is renamed
* An Emoji is replaced \(Using Pepe Manager Commands\)

If you need any more assistance with Pepe Manager, check out the rest of this documentation or join our support server to talk to an actual human!



### 

