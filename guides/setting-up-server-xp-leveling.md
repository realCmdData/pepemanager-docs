---
description: 'Reward your users activity with levels, role rewards and more!'
---

# Setting Up Server XP/Leveling

### Why Would You Need This?

Server Leveling is a super easy and effective way to ensure activity and growth in your Discord server. By setting out goals of activity with rewards, users will be enticed to keep the chat going to reach this goal you've put out for them. This goal can be anything from something as simple and inexpensive as a role reward that grants the user a special permission like the ability to send and embed images, to rewarding the topmost active users on your Discord with Nitro!  
Pepe Manager offers a free and easy-to-use XP and Leveling system so you can keep user retention high, and costs low!

### Video Tutorial

If you are averse to long bouts of reading, we have created a video tutorial that should be easy to follow along:

{% embed url="https://youtu.be/H-x3\_94-T8E" %}

## Guide

### Toggling Levels

By default, Pepe Manager will not have leveling enabled. Any user activity that may have occurred before you enabled leveling has not been counted. You need to enable it to get started by typing the following command:

```text
p!config toggle levels
```

### Adding Allowed Channels

You can now add specific channels that users can gain XP in. The channels that you set will be the only channels in the server where users can gain XP. You can add multiple channels with the same command \(By including a space in between channels\) or you can also add channels one after another. To add channels you can type the following command:

Where **&lt; &gt;** implies a required parameter

```text
p!config set xpChannels <Channel/ChannelID/ChannelMention>
```

{% hint style="info" %}
You can set the channel by writing the name of the channel, using the channel ID or by simply mentioning the channel.  
If you write an incomplete channel name the bot will look for the next closest one.
{% endhint %}

{% hint style="success" %}
#### And That's It!

If you only want the very basic leveling setup, you are done now! If you want to go more in-depth and learn about many more features that you can use, carry on!  
  
_**ALL STEPS BEYOND THIS POINT ARE OPTIONAL**_
{% endhint %}

### Adding No XP Roles

You can now set specific roles to not gain XP, regardless of whether or not the user is in the appropriate leveling channel or not. It is also not important if the user has another role on top or below the role you set to not gain XP.   
This feature is quite useful if you do not want your staff to gain XP, or to make sure that Muted users do not gain XP, etc. To add a role you can type the following command:

Where **&lt; &gt;** implies a required parameter

```text
p!config set noXpRoles <Role/RoleID/RoleMention>
```

{% hint style="info" %}
You can set the role by writing the name of the role, using the role ID or by simply mentioning the role.  
If you write an incomplete role name the bot will look for the next closest one, this is useful if you have system emojis as part of your role name.
{% endhint %}

### Adding the Top XP Role

You can also reward a user for having the most XP by letting the bot assign a Top XP role. This role is given out at 00:00 UTC, and is only ever given to one person on the server. If a user had the Top XP role previously, it will be taken off of them.   
This feature is a quick and easy way to give users a long-term goal to work towards. It also helps if the Top XP role is hoisted quite high on the server list, and is given a prominent colour. To set the Top XP role, you can type the following command:

Where **&lt; &gt;** implies a required parameter

```text
p!config set topXpRole <Role/RoleID/RoleMention>
```

{% hint style="warning" %}
It is **highly** suggested that you also set the Top XP role as a No XP role aswell. Not doing so might lead to the situation that only one person ever recieves the Top XP role since during their day on the Top they keep gaining XP.  
By letting them not gain XP for a day gives other users time to catch up.
{% endhint %}

### Customizing the Level-Up Message

If you find the current Level-Up message to not suit your server style, or you simply want to spice it up a little, you can completely customize it! We currently only support raw text messages \(Not Embeds\)  
To set the Level-Up message you can type the following command:

Where **&lt; &gt;** implies a required parameter

```text
p!config set xpMessage <Message>
```

There are several **tags** you can include in your Level-Up message. These parameters will be replaced with the appropriate information when the Level-Up message is sent.  
  
_You must include the {} brackets in your message for the tags to show up!_

| Information | Parameter |
| :--- | :--- |
| User Mention \(@User\) | {user} |
| User Tag \(User\#1234\) | {user.tag} |
| Username \(User\) | {user.username\) |
| User Discriminator \(1234\) | {user.discriminator} |
| User ID \(99787644430475264\) | {user.id} |
| Server Name \(My Cool Server\) | {guild.name} |
| Server ID \(493351982887862283\) | {guild.id} |
| Level Reached \(5\) | {level} |

### Where to send the Level-Up Message

By default Pepe Manager will simply send the Level-Up message in the same channel where the user who Leveled-Up last spoke in, but this can sometimes be intrusive and can disrupt normal conversation. Not to worry though, as you can set where Pepe Manager will send the Level-Up message. To set this up, simply type the following command:

Where **&lt; &gt;** implies a required parameter

```text
p!config set xpResponseType <Type>
```

There are several response types you can choose one. You can only choose one at a time, and the Level-Up message you may have set up earlier will be carried over to each response type. 

| Where Will it be Sent? | Response Type |
| :--- | :--- |
| In the same channel as the user | channel |
| In the user's direct messages | dm |
| In a specific channel all the time | \#Channel |
| Nowhere; all messages are off | off |

### Adding Role Rewards

The main meat of Leveling: the role rewards. You can set up roles to be given out to users when they reach a specific Level. This can be used to simply indicate the users level with a role, give out special colours to users as they gain higher levels, give out permissions that can be earned through activity, and so much more.   
With the free version of Pepe Manager you can set up to 2 roles to be given out on the same Level, however overall there is no limit to how many roles you can set up.  
The premium limit is 10 roles for the same Level.

Where **&lt; &gt;** implies a required parameter

```text
p!config set xpRoles <Level> <Role/RoleID/RoleMention>
```

{% hint style="info" %}
Please note that if your role contains multiple words, such as the role **Cool Person**, you must either use the Role ID or Mention, or only write the word **Cool**.  
  
The bot will see the words **Cool** and **Person** as separate roles.
{% endhint %}

### Automatically Resetting Levels

Automatically resetting levels can be very useful to keep your server nice and organized, and to punish those you ban even more!  
When the condition you set has been met, Pepe Manager will automatically the affected users level data \(If they had any\) without questions. **Kicking a user has the same effect as leaving though, so please be careful!**

Where  **&lt; &gt;** implies a required parameter

```text
p!config set autoResetLevels <Type>
```

There are several response types you can choose one. You can only choose one at a time.

| What Will Trigger the Reset? | Response Type |
| :--- | :--- |
| Nothing | none |
| When the user leaves the server for whatever reason | leave |
| When the user is banned for whatever reason | ban |
| When the user leaves or when the user is banned | both |

### Toggling Role Stacking

Now that you've set up some role rewards, you can choose whether or not the bot will stack the roles or not. Stacking means that each additional role reward will simply be added to the users already existing roles. Non-Stacking means that any previous role reward roles will be removed when the user gains a new role. This does not affect roles that are not specifically marked as rewards.  
By default, stacking is turned **on**.

```text
p!config toggle stackXpRoles
```

### Final Words

It's really easy to set up an activity tracking system, but as you want to add more and more features, and reward your users for the loytalty and acitvity it becomes more and more complex. If you are new to bots don't be scared of all of the complicated commands and command structures, new words that bots use to describe what they're doing, etc.  
Bots can be a fantastic tool to build a great community, and learning the inner workings of a bot you are going to be spending a lot of time with anyway can prove useful later on.

