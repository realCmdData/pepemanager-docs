---
description: Learn how Pepe Manager can automatically celebrate a milestone with you!
---

# Automatically Controlled Member Milestones

### Why Would You Need This?

Celebrating a member milestone is a super simple and social activity. Whether you're celebrating 100 members or 100,000, it's just as a momentous occasion as any. By celebrating and rewarding the user who joined as your nth member, you can always set a new goal to reach, a new level of growth to achieve. Automating this process is quick and simple, and the possibilities are endless!

### Video Tutorial

If you are averse to long bouts of reading, we have created a video tutorial that should be easy to follow along:

{% embed url="https://youtu.be/nXlhdcH3YaU" %}



## Guide

### Enabling Milestones

The first step is to enable the milestone feature in your Pepe Manager settings. This acts as a useful switch if you want to stop using milestones, but want to keep all of your configured settings we will get into later on. To enable it, type the following command:

```text
p!config toggle milestones
```

### Setting the Milestones Channel

The next step is to set a milestones channel, where all of your automated milestone announcements will be sent in! This can be a regular text channel or if you have a community enable server, this can also be an announcement channel. To set your channel, type the following command:

Where **&lt; &gt;** implies a required parameter

```text
p!config set milestonesChannel <Channel/ChannelID/ChannelMention>
```

### Setting the Milestones Interval

This next step is quite an important one because now you can choose at what member count you want your milestone to be triggered at. The interval is the number of members between each milestone, and by default it is set to **100**. This means that every 100 members, a milestone is triggered, such as **200**, **300**, **400**, etc.  
The milestone interval can be any number within reason as long as it is a _**multiple of 5**_. Conceivably the interval can be set to **5** or it can be set to **100,000**. To set your interval, type the following command:

Where **&lt; &gt;** implies a required parameter

```text
p!config set milestonesInterval <Number>
```

### Setting the Milestones Message

Next up you can also customize your milestone message, which is the message that is sent when a milestone is reached. By default the message looks as follows:

![](https://i.imgur.com/IUZMJGP.png)

You may include any number of emojis \(As long as the bot can access them\), formatting, line breaks, special characters and even role mentions as long as it is within the 2000 character limit of all messages. To set your milestone message, type the following command:

Where **&lt; &gt;** implies a required parameter

```text
p!config set milestonesMessage <Message>
```

{% hint style="warning" %}
If you are including a role mention in your message, make sure that Pepe Manager has permission to mention that role, otherwise it won't work and the message might turn out looking very ugly.
{% endhint %}

There are several **tags** you can include in your Milestone message. These parameters will be replaced with the appropriate information when the Milestone message is sent.  
  
_You must include the {} brackets in your message for the tags to show up!_

| Information | Tag |
| :--- | :--- |
| User Mention \(@User\) | {user} |
| User Tag \(User\#1234\) | {user.tag} |
| Username \(User\) | {user.username\) |
| User Discriminator \(1234\) | {user.discriminator} |
| User ID \(99787644430475264\) | {user.id} |
| Server Name \(My Cool Server\) | {guild.name} |
| Server ID \(493351982887862283\) | {guild.id} |
| Milestone Achieved \(100\) | {milestone} |

### Setting the Milestones Role

Lastly you can also reward users who conveniently joined at exactly the right time by granted them a role or several. Free servers can set up to **5** roles to be given out to that special someone, and [Premium ](../information/patreon-perks.md)servers can set up to **10** roles. To set your milestone role\(s\), type the following command:

Where **&lt; &gt;** implies a required parameter

```text
p!config set milestonesRole <Role/RoleID/RoleMention>
```

### Final Words

And that's it! You've successfully created Automatically Assigning Roles with Pepe Manager!

If you need any more assistance with Pepe Manager, check out the rest of this documentation or join our support server to talk to an actual human!

