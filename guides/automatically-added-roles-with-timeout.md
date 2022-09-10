---
description: >-
  Learn how Pepe Manager can automatically assign new users roles without
  breaking the Discord verification system!
---

# Automatically Adding Roles (With Timeout)

### Why Would You Need This?

Automatically adding roles to new members can serve many useful purposes, from giving new members a cool colour in your chat, to giving out permission roles that can be taken away if needed, or for adding ping roles for announcements.\
However, if you have a Discord verification level enabled that makes users who don't surpass the verification level needed, automatically adding a role when someone joins will bypass this verification filter! Pepe Manager allows you to set a timer from the moment a user joins to when they will receive the role, so the verification system is not bypassed!

### Video Tutorial

If you are averse to long bouts of reading, we have created a video tutorial that should be easy to follow along:

{% embed url="https://youtu.be/94NleboBP_o" %}

## Guide

### Evaluating your Verification Level

In order for this guide to be most effective, you should go into your server settings, go to the Moderation tab, and double-check which verification level you have selected.

![](https://i.imgur.com/dZ9o0ae.png)

The verification level of **Medium** has a timeout of 5 minutes, whereas the **High** and **Highest** settings have a timeout of 10 minutes.

### Setting your Autoroles

You can now add your autoroles to Pepe Manager. In the current version, it is not possible to assign different roles to different timeouts, they will all be assigned at the same time.\
The free version of the bot allows you to assign up to 5 autoroles at the same time, whereas the premium allows you to assign up to 25 autoroles. [Click here to learn more](../information/patreon-perks.md).

Where **< >** implies a required parameter

```
p!config set autoRole <Role/RoleID/RoleMention>
```

{% hint style="warning" %}
You can set all of your autoroles with the same command simply by putting a space between each role, however, this only works for Role Mentions and Role ID's if one or more of the roles you want to assign have a space in their name.\
Spaces are treated as separators, and if you enter the full role name with a space, Pepe Manager will treat them as 2 separate roles.
{% endhint %}

### Setting your Timeout

You can now specify how long the bot should wait before assigning the roles after a user joins. This is not limited to either 5 minutes or 10 minutes, you can set the timeout to as little as 1 minute or as high as 30 minutes.

Where **< >** implies a required parameter

```
p!config set autoRoleTimeout <Time>
```

### Final Words

And that's it! You've successfully created Automatically Assigning Roles with Pepe Manager!

If you need any more assistance with Pepe Manager, check out the rest of this documentation or join our support server to talk to an actual human!

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}
