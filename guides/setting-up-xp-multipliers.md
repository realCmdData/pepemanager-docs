---
description: Verander wie hoeveel XP krijgt, en waar!
---

# Het opzetten van XP Multipliers

### Waarom zou u dit nodig hebben?

Met Pepe Manager kunt u verschillende XP vermenigvuldigers instellen, en u kunt ze voor verschillende gebruikers in verschillende situaties laten gelden om verschillende dingen te belonen! Een veel voorkomende toepassing is het belonen van Boosters met een hogere XP vermenigvuldiger! U kunt ook uw hele server vermenigvuldiger veranderen als u denkt dat mensen een beetje te snel levelen naar uw smaak, of u kunt ook meer XP geven in kanalen waar mensen misschien niet vaak praten!

### Video handleiding

Op dit moment hebben we nog geen video handleiding voor deze gids, kom later terug!

## Handleiding

### Zorg ervoor dat je leveling hebt ingesteld

Voordat u deze gids volgt, moet u er zeker van zijn dat u het levelen in uw server al goed hebt ingesteld. Als je daar hulp bij nodig hebt, volg dan onze gids hier:

{% page-ref page="setting-up-server-xp-leveling.md" %}

### Multipliers begrijpen

Aan vermenigvuldigingsfactoren moet je misschien even wennen, maar maak je geen zorgen! Daar is deze gids voor! Vermenigvuldigers nemen het aantal XP dat een gebruiker normaal voor een geldig bericht zou krijgen, en vermenigvuldigen dit met het aantal dat op de vermenigvuldiger is ingesteld. Bijvoorbeeld als een gebruiker `34` XP krijgt voor een bericht, maar de server heeft een globale vermenigvuldiger van x1.5, dan zal hij in feite `51` XP krijgen.    
  
Echter, vermenigvuldigers kunnen ook lager dan 1 worden ingesteld, wat betekent dat een vermenigvuldiger van x0.5 geldig is, maar dat betekent niet een 50% XP winst, maar eerder een 50% XP verlies. **Elke vermenigvuldiger die hoger is dan 1 zal meer XP geven, en elke vermenigvuldiger die lager is dan 1 zal XP wegnemen.**

{% hint style="info" %}
Als je liever in percentages denkt: een vermenigvuldiger van x1,5 staat gelijk aan 150% XP-winst, en een vermenigvuldiger van x3,4 staat gelijk aan 340% XP-winst.
{% endhint %}

### De hiërarchie begrijpen

Wanneer u meer dan één vermenigvuldiger actief hebt, wordt een hiërarchie opgesteld om te beslissen welke vermenigvuldiger in welke omstandigheid wordt gebruikt. De hiërarchie van de rolvermenigvuldigers is een beetje anders en zal in [deze sectie] worden uitgelegd (https://docs.pepemanager.com/guides/setting-up-xp-multipliers#changing-role-multiplier-hierarchy).

Stel dat we een globale multiplicator van x1.1 hebben, een kanaalmultiplicator van x1.5 in \#kanaal-A, een kanaalmultiplicator van x0.75 in \#kanaal-B en nog een \#kanaal-C zonder multiplicator:

| Vermenigvuldiger | Toepassing |
| :--- | :--- |
| x1.1 | Global |
| x1.5 | \#Kanaal-A |
| x0.75 | \#Kanaal-B |
| Geen | \#Kanaal-C |

Op basis hiervan willen we nu weten welke vermenigvuldigingsfactor in elk kanaal zal worden gebruikt.  
Als we in \#kanaal-A praten, zal de vermenigvuldigingsfactor van kanaal-A worden gebruikt, omdat dit de hoogste is die momenteel van toepassing is.  
Als we in \#kanaal-B praten, wordt de globale vermenigvuldigingsfactor gebruikt, omdat de kanaal-vermenigvuldigingsfactor lager is dan de globale vermenigvuldigingsfactor.  
Als we in \#kanaal-C praten, wordt de globale vermenigvuldigingsfactor gebruikt, omdat er helemaal geen kanaal-vermenigvuldigingsfactor is ingesteld.

{% hint style="success" %}
Indien van toepassing, wordt altijd de hoogste vermenigvuldigingsfactor gebruikt!
{% endhint %}

### Globale vermenigvuldigers instellen

Globale vermenigvuldigers zijn, zoals de naam al zegt, van toepassing op de hele server, ongeacht rol, kanaal, permissies, enz. Ze kunnen nuttig zijn wanneer je de totale XP winst op je server wilt regelen, bijvoorbeeld als je vindt dat je leden een beetje te snel XP winnen, het introduceren van een globale vermenigvuldiger die kleiner is dan 1 zal de hoeveelheid XP die globaal wordt gewonnen verlagen. Om een globale vermenigvuldiger toe te voegen, kun je het volgende commando typen:

Waar **&lt; &gt;** een verplichte parameter inhoudt

```text
p!config set xpMultiplier global <Multiplier>
```

{% hint style="info" %}
Met Global Multipliers kun je de levelcurve aanpassen aan die van andere populaire bots!  
_Uitgaande van standaard XP opties & Multipliers_  
  
**AmariBot •** x0.09  
**Atlas •** x0.22  
**Arcane •** x0.87  
**MEE6 •** x0.65 
{% endhint %}

### Kanaal-vermenigvuldigers instellen

Met kanaalvermenigvuldigers kunt u per kanaal een vermenigvuldigingsfactor instellen, maar u kunt ook meerdere kanalen op dezelfde vermenigvuldigingsfactor instellen, of verschillende vermenigvuldigingsfactoren voor verschillende kanalen instellen! Om een kanaal-vermenigvuldigingsfactor toe te voegen, kun je het volgende commando typen:

Waar **&lt; &gt;** een verplichte parameter inhoudt

```text
p!config set xpMultiplier channel <Multiplier> <Channel/ChannelID/ChannelMention>
```

### Rol-vermenigvuldigers instellen

Rollenmultipliers werken op dezelfde manier als kanaalmultipliers. U kunt verschillende rollen aan dezelfde vermenigvuldiger toewijzen of verschillende vermenigvuldigers voor verschillende rollen maken! Om een rol vermenigvuldiger toe te voegen, kun je het volgende commando typen:

Waar **&lt; &gt;** een verplichte parameter impliceert

```text
p!config set xpMultiplier role <Multiplier> <Role/RoleID/RoleMention>
```

### Rolvermenigvuldigingshiërarchie veranderen

Als u nog niet gelezen hebt hoe de gewone vermenigvuldigingshiërarchie werkt, lees dan eerst [die sectie](https://docs.pepemanager.com/guides/setting-up-xp-multipliers#understanding-the-hierarchy).

Rolhiërarchie **wordt standaard** op dezelfde manier beheerd als alle andere vermenigvuldigers; de hoogste toepasselijke vermenigvuldiger zal worden gebruikt **ongeacht** de rolhiërarchie. Je kunt echter de prioriteit van welke vermenigvuldiger wordt gebruikt wijzigen door dit aan te vinken in de configuratie.   
Als je dat doet, wordt de hoogste rol van een gebruiker gebruikt waaraan ook een vermenigvuldigingsfactor is gekoppeld, zelfs als een lager geplaatste rol een hogere vermenigvuldigingsfactor heeft. Om de prioriteit van de rolhiërarchie in te stellen, kunt u het volgende commando gebruiken:

```text
p!config toggle prioritiseMultiplierRoleHierarchy
```



