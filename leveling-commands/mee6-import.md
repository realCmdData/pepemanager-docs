# MEE6 Import

### Description

This command can be used to import any existing MEE6 leveling database that may exist for your server. In order for this to work, the MEE6 bot needs to still be in your server and the leveling plugin in the MEE6 dashboard still needs to be on.

By default will only import users down to level 5 to save on API requests, however if you run a much smaller server, you can use the optional command tag to lower this threshold down to level 3. Any users below this level will simply not be imported.

The command only imports XP numbers, however it will convert the XP into the appropriate MEE6 equivalent level numbers using MEE6's own leveling algorithm. After the conversion the leveling progression will follow Pepe Manager's own leveling algorithm.

This command has a strict cooldown limit on it to prevent our bot from being rate-limited from the MEE6 API. Please only use this command sparingly.

You may also import the database over from another server if you are the owner of both the old \(To be imported from\) and the new \(To be imported into\) servers.

### Command Structure

Where **\[ \]** implies an optional parameter  
Where **--Until** implies a command tag

```text
p!mee6import [ServerID] [--Until]
```

The command tags need to be used as an addition to the command:

```text
[--Until] = --Until [MEE6 Level]
```

### **Permission**

* `Server Owner`**\(User\)**
* N/A **\(Bot\)**

### Aliases

* `mee6_import`
* `meesix_import`

