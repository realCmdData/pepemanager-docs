---
description: >-
  Prepare Lurkr for observation. This guide covers the initial steps to get
  Lurkr tracking activity and rewarding your members.
---

# 📈 Initial Leveling Setup

## Guide

### Coming From A Different Bot?

Are you switching to Lurkr from a different leveling bot which you've already used extensively? We understand that resetting your servers leaderboard is something you'd rather never do, and setting up leveling role rewards from scratch is a hassle as well.&#x20;

Why not check out how to automatically import levels from other bots? If the bot you're coming from is supported, Lurkr can pick up where you left off just moments ago!

{% content-ref url="importing-levels-from-other-bots.md" %}
[importing-levels-from-other-bots.md](importing-levels-from-other-bots.md)
{% endcontent-ref %}

***

### Toggling Levels

By default, Lurkr will not have leveling enabled. Any user activity that may have occurred before you enabled leveling has not been counted. You need to enable it to get started by typing the following command:

<figure><img src="https://i.imgur.com/h5OlJcV.png" alt=""><figcaption></figcaption></figure>

### What Messages Count for Leveling?

Any of the following messages can count towards leveling progression, provided the member is not blocked from leveling in some way or another.

* Default text messages
* Reply text messages
* Slash command usages (Any bot, non-ephemeral)
* Context menu command usages (Any bot, non-ephemeral)

***

### Adding Leveling Channels

You can now add specific channels that users can gain XP in. The channels you setup will be by default blacklisted channels, meaning that they are the only ones that are excluded from being able to gain XP.&#x20;

However, as we will explain shortly you can very easily change that within moments. For now, use the /config set command to add as many channels as you want!

You can enter as many channels as your current server plan will allow. You can check the limits on the Patreon Perks page!

{% content-ref url="../information/patreon-perks.md" %}
[patreon-perks.md](../information/patreon-perks.md)
{% endcontent-ref %}

<figure><img src="https://i.imgur.com/c2lArsP.png" alt=""><figcaption><p>You can add up to 30 channels for free, or 50 channels with <a href="../information/patreon-perks.md">Premium</a>!</p></figcaption></figure>

Now the bot will send a confirmation message of the information you just entered, however included with that is also a grey button that let's you toggle between the blacklist and the whitelist option whilst still retaining all of the channels you just set! If you therefore want **only** the channels you just entered to be used as leveling channels, press the button that says 'Switch to whitelist'

<figure><img src="https://i.imgur.com/BTQJKQA.png" alt=""><figcaption><p>If you don't do anything, the channels will be set as they are!</p></figcaption></figure>

{% hint style="info" %}
To simply things and help you understand the different leveling channel modes here is an overview:

**Whitelist** enabled & no leveling channels set = Members **can't** gain levels anywhere

**Blacklist** enabled & no leveling channels set = Members **can** gain levels everywhere
{% endhint %}

***

{% hint style="success" %}
#### And That's It!

If you only want the very basic leveling setup, you are done now! If you want to go more in-depth and learn about many more features that you can use, continue with the next guide!
{% endhint %}

{% content-ref url="customize-level-up-messages.md" %}
[customize-level-up-messages.md](customize-level-up-messages.md)
{% endcontent-ref %}

