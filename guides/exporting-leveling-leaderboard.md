---
description: Learn how to export your Pepe Manager leaderboard into a tangible file!
---

# Exporting Leveling Leaderboard

### Why Would You Need This?

Well, we seriously hope you really really **DON'T** need this, surprisingly! We want to make Pepe Manager as accessible, feature-full and easy to use as no bot before it!\
\
The reason we implemented an export feature is to essentially **not be an asshole** and lock you dear user into a bot that you realistically cannot remove without great detriment to your community by taking away all of the months or even years of leveling grinding your users have already done.

## Guide

### File Structure

Below is an example of what the file structure of your leveling leaderboard export will look like,

```javascript
interface Level {
    avatar: string | null;
    level: number;
    tag: string | null;
    userId: string;
    xp: number;
}

interface Export {
    levels: Level[];
}
```
