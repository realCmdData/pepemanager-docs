---
description: Learn how to automatically control who can mention a certain role!
---

# Automatic Role Mention Cooldown

### Why Would You Need This?

The main use-case of this feature is to have a moderator role mention cooldown. Many servers like to keep their Moderator role mentionable in case some accident or disaster happens to keep moderators on stand-by ASAP. However, if this power is given to too many people, eventually there will be people who abuse this and spam ping moderators constantly, even when there is no emergency.

### Video Tutorial

We currently do not have a video tutorial for this guide just yet, check back later!

## Guide

### Setting up the roles

In order to get started, first, you must set which roles will have a mention cooldown. Typically this will be the moderator role or the administrator role, however, it is entirely up to you which role\(s\) you decide to choose. To set your role\(s\), type the following command:

Where **&lt; &gt;** implies a required parameter

```text
p!config set mentionCooldownRoles <Role/RoleID/RoleMention>
```

### Setting up the cooldown time

The cooldown time can be any time between 5 minutes and 30 minutes, and it is the time between when the role mention option is disabled after a mention in a channel to when it is re-enabled. To set your cooldown time, type the following command:

Where **&lt; &gt;** implies a required parameter

```text
p!config set mentionCooldown <Time>
```

### Final Words

And that's it! You've successfully created automatic role mention cooldowns with Lurkr!

If you need any more assistance with Lurkr, check out the rest of this documentation or join our support server to talk to an actual human!

