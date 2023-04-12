---
description: Let Lurkr take the reigns, completely hassle-free!
---

# 📀 Importing Levels From Other Bots

### Why Would You Need This?

Server Leveling can be a painful transition for already set-up servers, and is very often a pain point when server owners/admins want to looking for a different leveling solution. Lurkr allows you to import all levels and role rewards from various supported bots and keep your users leveling data completely intact, so they don't have to start from scratch all over again!

### Video Tutorial

We currently do not have an updated video tutorial for this guide just yet, check back later!

## Guide

### Important Information

{% hint style="danger" %}
**Please read this section before moving forward to prevent data-loss and unnecessary waiting during the transition!**

While Lurkr lets you painlessly import all of your leveling data, this feature requires significant processing power. Not only that but we are obligated to retrieve data from other bots within their rate-limits (ie. How fast we can access their website). Because of this, the `/importxp` command can only be used **once every hour**!&#x20;

It is therefore important to read through this guide carefully before proceeding!
{% endhint %}

### Supported Bots

Not all bots are open with their leveling data so that these kinds of transfers are possible. Below is a list of supported bots that allow for our importing feature to work. Below is also a list of bots that **we know** are not compatible because they require special authorization on your behalf to access the leaderboard. Since we would never ask for your Discord credentials, unless these bots change their policies in the future, we **cannot** support them.

|               Bot              |    Leveling Import?   |  Role Reward Import?  |
| :----------------------------: | :-------------------: | :-------------------: |
|    [MEE6](https://mee6.xyz)    |           ✅           |           ✅           |
|   [Atlas](https://atlas.bot)   |           ✅           |           ✅           |
|  [Arcane](https://arcane.bot/) |   ❌ (Not Supported)   |   ❌ (Not Supported)   |
| [Amari](https://amaribot.com/) | ❔(API Access Unclear) | ❔(API Access Unclear) |

If you want to see this list get expanded, let us know which bot you would like to switch over from in our support server in the #suggestions channel! We'll let you know if it's technically possible and if enough people are interested, add it to our feature request list!



### Import Levels

#### Choose a Bot

Lets get started on importing your levels to Lurkr! In order to use the command the person executing it needs to have **Administrator** permission, or be the owner of the server!

To start, enter the `/importxp` command and wait for the option fields to be populated. You will now have an option to choose one of the above supported bots!

<figure><img src="https://i.imgur.com/V7zolEQ.png" alt=""><figcaption></figcaption></figure>

#### Role Rewards

Click on one of the supported bots, in this guide we will be using MEE6 as an example. Next you will need to choose whether or not to import role rewards. If you already had some role rewards set up, most likely the answer will be yes, unless you plan on re-doing your role rewards.&#x20;

{% hint style="info" %}
Since importing role rewards **only** transfers the information which Discord role belongs to which level, the bot should not create or move around existing roles.&#x20;
{% endhint %}

Click on **True** in order to import the role rewards, or **False** if you just want to import the levels.

<figure><img src="https://i.imgur.com/QVYwDPA.png" alt=""><figcaption></figcaption></figure>

#### Until Option

Lastly, you will be prompted with an 'until' option. This **optional** field lets you control down to which level you want to import your users.&#x20;

For example, if you have a lot of users who are all on level 1 because they only ever spoke 2 words in your server, the import will skip them entirely. This is mainly useful for large servers (Over \~1,000 members) who might have a lot of unnecessary users in their leveling leaderboard. This helps reduce the overall processing the bot needs to do.

The **lowest** this value can go is `3`, meaning that if you select `until:3`, Lurkr will import all levels until it reaches level 3 and will then stop importing. The **highest** this value can go is `20`.

{% hint style="info" %}
By default, the `until` value is set to 5.
{% endhint %}

<figure><img src="https://i.imgur.com/nMSotqw.png" alt=""><figcaption></figcaption></figure>

#### Success?

Once you've sent the command away, Lurkr will now collect all of the relevant data from your old bot and transfer it all into it's own database. The reply message will update to keep you apprised of the transfer progress.&#x20;

Once it has finished the message should look like this, and you will be able to use the `/leaderboard` command or the `/config check` command to double-check if all of your data has been moved over!

<figure><img src="https://i.imgur.com/px2NXLp.png" alt=""><figcaption></figcaption></figure>

#### Are We Hypocrites?

So we've stolen all of your leveling data and are now holding it hostage until you pay us right? _**WRONG!**_

We believe in vastly different philosophy than our competitors and as end-users of these kinds of systems ourselves in the past, we understand the pain and frustrations some of the other options give you.

All of which is why we allow you to export/download your leveling data at **any time**, **instantly** and completely for free! Check out how in the guide linked below!

{% content-ref url="exporting-leveling-leaderboard.md" %}
[exporting-leveling-leaderboard.md](exporting-leveling-leaderboard.md)
{% endcontent-ref %}

### Final Words

Congratulations, you should now be the proud owner/administrator of a brand newly imported leveling system powered by Lurkr!

{% hint style="danger" %}
If you experienced any issues in this process, please feel free to seek support in our support server linked below!
{% endhint %}

{% embed url="https://discord.com/invite/XUQAnkq2vy" %}

{% hint style="success" %}
If everything went according to plan, check out all of our awesome **free** features that you might like to configure for your personal leveling experience!
{% endhint %}

{% content-ref url="setting-up-server-leveling.md" %}
[setting-up-server-leveling.md](setting-up-server-leveling.md)
{% endcontent-ref %}
