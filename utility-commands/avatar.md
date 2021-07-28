# Avatar

### Description

This command can be used to display the avatar of yourself or of other users. You can change the size of the avatar that is displayed and even change the format in which it's saved, useful for example for converting GIF avatars to still images.

The command can fetch the avatar of any user on Discord as long as you provide it with a User ID if the user is not in a shared server.

### Command Structure

Where **\[ \]** implies an optional parameter  
Where **--Size** implies a command tag   
Where **--Format** implies a command tag

```text
p!avatar [User] [--Size] [--Format]
```

The command tags need to be used as an addition to the command:

```text
[--Size] = --Size [Number]
[--Format] = --Format [Type]
```

Below is a table containing all valid tag parameters that can be used in conjunction with a tag.

| **--Size** | --Format |
| :--- | :--- |
| 16 | PNG |
| 32 | JPG |
| 64 | JPEG |
| 128 | GIF |
| 256 | WEBP |
| 512 |  |
| 1024 |  |
| 2048 |  |
| 4096 |  |

### **Permission**

* N/A **\(User\)**
* `Embed Links`**\(Bot\)**

### Aliases

* `avatar`
* `av`

