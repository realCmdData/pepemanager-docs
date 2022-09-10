---
description: Change who gains how much XP, and where!
---

# Setting Up XP Multipliers

### Why Would You Need This?

With Pepe Manager you can control various different XP multipliers, and you can let them apply to different users in different situations to reward different stuff! A very common use-case is the rewarding of Boosters with a higher XP multiplier! You can also change your entire server multiplier if you think people are leveling up a bit too quickly for your liking, or you can also give more XP in channels where people might not talk often!

### Video Tutorial

We currently do not have a video tutorial for this guide just yet, check back later!

## Guide

### Make sure you have leveling set up

Before following this guide, please make sure that you have correctly set up leveling in your server already. If you need guidance in doing so, please follow our guide here:

{% content-ref url="setting-up-server-xp-leveling.md" %}
[setting-up-server-xp-leveling.md](setting-up-server-xp-leveling.md)
{% endcontent-ref %}

### Understanding Multipliers

Multipliers might take some getting used to, but don't worry! That's what this guide is for! Multipliers essentially take the amount of XP a user would normal receive for a valid message, and multiply it by however much the multiplier is set to. For example if a user gains `34` XP for one message, but the server has a global multiplier of x1.5, they will actually receive `51` XP.  \
\
However, multipliers can also be set below 1, meaning a multiplier of x0.5 is valid, but that does signify a 50% XP gain, but rather a 50% XP loss. **Any multiplier that is above 1 will give more XP, and any multiplier that is below 1 will take away XP.**

{% hint style="info" %}
If you prefer to think in percentages; a multiplier of x1.5 equals a 150% XP gain, and a multiplier of x3.4 equals a 340% XP gain.
{% endhint %}

### Understanding the Hierarchy

When you have more than one multiplier currently active, a hierarchy is established to decide which multiplier is used in which circumstance. Role multiplier hierarchy is a bit different and will be explained in [this section](https://docs.pepemanager.com/guides/setting-up-xp-multipliers#changing-role-multiplier-hierarchy).

Lets say that we have a global multiplier of x1.1, a channel multiplier of x1.5 in #Channel-A, a channel multiplier of x0.75 in #Channel-B and another #Channel-C with no multiplier:

| Multiplier | Application |
| ---------- | ----------- |
| x1.1       | Global      |
| x1.5       | #Channel-A  |
| x0.75      | #Channel-B  |
| None       | #Channel-C  |

Based on this, we now want to know what multiplier will be used in each channel.\
If we talk in #Channel-A, the multiplier of #Channel-A will be used, since it is the highest one currently applicable.\
If we talk in #Channel-B, the global multiplier will be used, since the channel multiplier is lower than the global one.\
If we talk in #Channel-C, the global multiplier will be used, since there is no channel multiplier set at all.

{% hint style="success" %}
Whenever applicable, the highest multiplier will always be used!
{% endhint %}

### Setting Global Multipliers

Global multipliers, as the name suggests, apply to the entire server regardless of role, channel, permissions, etc. They can be useful when you want to regulate the total XP gain on your server, for example if you find that your members are gaining XP a bit too quickly, introducing a global multiplier that is less than 1 will lower the amount of XP gained globally. To add a global multiplier, you can type the following command:

<figure><img src="../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

A modal-box will then appear, in which you can then enter the global multiplier you want to assign.

{% hint style="info" %}
Using Global Multipliers you can change the leveling curve to match that of other popular bots!\
&#x20;_\*Assuming Default XP Options & Multipliers_\
__\
__**AmariBot •** x0.09\
**Atlas •** x0.22\
**Arcane •** x0.87\
**MEE6 •** x0.65&#x20;
{% endhint %}

### Setting Channel Multipliers

Channel multipliers allow you to set multipliers on a per-channel basis, but not only that, they also let you set multiple channels to the same multiplier, or set different multipliers for several channels! To add a channel multiplier, you can type the following command:

<figure><img src="../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

A modal-box will then appear, in which you can then enter the global multiplier you want to assign.

### **Setting Role Multipliers**

Role multipliers work in much the same way as channel multipliers. You can assign numerous roles to the same multiplier, or create different multipliers for different roles! To add a role multiplier, you can type the following command:

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

A modal-box will then appear, in which you can then enter the global multiplier you want to assign.

### Changing Role Multiplier Hierarchy

If you haven't read how the regular multiplier hierarchy works, please read [that section](https://docs.pepemanager.com/guides/setting-up-xp-multipliers#understanding-the-hierarchy) first.

Role hierarchy **by default** is managed in the exact same way as all other multipliers; the highest applicable multiplier will be used **regardless** of the role hierarchy. However, you can change the prioritization of which multiplier is used by toggling it in the config. \
If you do so, the highest role that a user has that also has a multiplier attached to it will be used, even if a lower ranking role has a higher multiplier. To toggle role hierarchy prioritization, you can type the following command:

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

### Final Words <a href="#final-words" id="final-words"></a>

And that's it! You've successfully learned how to use XP Multipliers in Pepe Manager!

If you need any more assistance with Pepe Manager, check out the rest of this documentation or join our support server to talk to an actual human!

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}
