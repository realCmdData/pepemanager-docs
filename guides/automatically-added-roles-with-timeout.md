---
description: >-
  Learn how Lurkr can automatically assign new users roles without breaking the
  Discord verification system!
---

# 📬 On Join Roles

### Why Would You Need This?

On Join roles are super useful in order to give new users certain roles, or to give users with special profile badges roles automatically! Lurkr also lets you set a timer before giving these roles so that your Discord Verification system doesn't immediately break!

### Video Tutorial

We currently do not have a video tutorial for this guide just yet, check back later!

## Guide

### Evaluating your Verification Level

In order for this guide to be most effective, you should go into your server settings, go to the Moderation tab, and double-check which verification level you have selected.

![](https://i.imgur.com/dZ9o0ae.png)

The verification level of **Medium** has a timeout of _5 minutes_, whereas the **High** and **Highest** settings have a timeout of _10 minutes_.

By assigning a role immediately after a user joins, the verification level doesn't apply to them.

Therefore in order for the verification level to still apply, it is advised to set the On Join timeout to the same time as the verification level when we get to that part!

### Setting your On Join Roles

You can now add your On Join Roles to Lurkr. In the current version, it is not possible to assign different roles to different timeouts, they will all be assigned at the same time.

You can enter as many roles as your current server plan will allow. You can check the limits on the Patreon Perks page!

{% content-ref url="../information/patreon-perks.md" %}
[patreon-perks.md](../information/patreon-perks.md)
{% endcontent-ref %}

<figure><img src="https://i.imgur.com/ri6nUsZ.png" alt=""><figcaption></figcaption></figure>

### Setting your Timeout

You can now specify how long the bot should wait before assigning the roles after a user joins. This is not limited to either 5 minutes or 10 minutes, you can set the timeout to as little as 1 minute or as high as 30 minutes.

<figure><img src="https://i.imgur.com/i3SsTZi.png" alt=""><figcaption></figcaption></figure>

A modal-box will then appear, in which you can then enter the time interval you want to assign.

<figure><img src="https://i.imgur.com/fgIdB09.png" alt=""><figcaption></figcaption></figure>

### Setting Badge-Specific On Join Roles

Rather than manually assigning roles to everyone who joins and has a specific profile badge, like the 3 Hypesquad Houses or a Discord Partner badge, let Lurkr do all the work for you!

To get started, type the command below, with the role you want to assign to **one badge** as the values option as shown below.

<figure><img src="https://i.imgur.com/pi6155A.png" alt=""><figcaption></figcaption></figure>

After entering which role(s) you want to assign specific profile badges, you will get a drop-down menu from which you can select any and all profile badges.

<figure><img src="https://i.imgur.com/h8aoUBY.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Discord bots can't see paid badges, eg. Nitro or Boost. Therefore we can't reliably tell whether or not a user has that badge and can't therefore be assigned a role.
{% endhint %}

### Final Words

And that's it! You've successfully created On Join Roles with Lurkr!

If you need any more assistance with Lurkr, check out the rest of this documentation or join our support server to talk to an actual human!

{% embed url="https://lurkr.gg/support" %}
