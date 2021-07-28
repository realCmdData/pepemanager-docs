# Set

### Description

{% hint style="warning" %}
This is a **method** or **sub-command** of the [Background ](./)command. It is not its own command.
{% endhint %}

This method of the [background ](./)command can be used to set a leveling background if none has been set yet, or can also be used to replace an existing custom leveling background with a new one.

Your custom background needs to have an aspect ratio of **4:1**, to fit into the leveling card. The bot will tell you if the image you have provided is inadequate. If your image only strays sightly from the required aspect ratio, the bot will try to compensate and cut off any excess to make the image fit.

For the best possible result we recommend that you crop your image manually to fit the aspect ratio before setting it.

{% hint style="info" %}
The **set** method is the default method when you simply run the background command. Running the background command with an image attached will acomplish the same thing.
{% endhint %}

{% hint style="danger" %}
The bot cannot check the uploaded images for NSFW content! If you want your users to not upload NSFW content to their leveling background, we suggest moderating the commands channel!
{% endhint %}

### Command Structure

Where **&lt; &gt;** implies a required parameter

```text
p!background set <AttachedImage/ImageURL>
```

### **Permission**

* `Attach Files` **\(User\)**
* N/A **\(Bot\)**

### Aliases

* N/A

