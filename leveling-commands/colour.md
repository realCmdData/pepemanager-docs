# Colour

### Description

This command can be used to change the colour of the progression bar in the [level ](rank.md)command. The colour change is global, no matter on which server you use the command.

By default, the progression bar is set to the **average** value, which will calculate the average colour of your profile picture and use it as the bar colour. If you have a GIF profile picture, it will calculate the average colour from the first frame.

You can also set the progression bar to the **role** value. This will take your top-most role that has a colour (Transparent roles, or roles with the "Default" colour don't count) and use it as the bar colour.

If you set this value the colour will change between servers, depending on the role colour that you have. If you don't have any roles, or only have transparent or "Default" roles, the bot will revert to using your profile picture to calculate an average value.

Lastly, you can also set the progression bar to a **custom colour** value. This lets you completely customize the bar colour to whatever colour you want, provided you give a correct [hex code](https://www.color-hex.com/).

{% hint style="info" %}
**Special Hint!**

If you set your rank progress colour to a hex code, it will also show up on the website leaderboard! [https://lurkr.gg/levels/](https://lurkr.gg/levels/)
{% endhint %}

### Command Structure

```
/colour <colour:>
```

| Value                   |                                                   Description |
| ----------------------- | ------------------------------------------------------------: |
| Hex Code (e.g. #2ecc71) |                Sets the colour to your custom hex colour code |
| Average                 | Sets the colour to the average colour of your profile picture |
| Role                    |       Sets the colour to the role colour of your highest role |

<figure><img src="https://i.imgur.com/UApCxnW.png" alt=""><figcaption></figcaption></figure>

### **Permission**

* N/A **(User)**
* N/A **(Bot)**
