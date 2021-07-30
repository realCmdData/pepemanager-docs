---
description: Leer hoe je aankondigingskanalen zo instelt dat ze zichzelf automatisch publiceren!
---

# Automatisch aankondigingen publiceren

### Waarom zou je dit nodig hebben?

Als je er nog niet van gehoord hebt, [Discord Announcement Channels](https://support.discord.com/hc/en-us/articles/360032008192-Announcement-Channels-) zijn een super handige toevoeging aan elke community server om hun bereik uit te breiden naar een publiek buiten je eigen server! Maar om dat te doen moet je handmatig op een kleine knop klikken om er zeker van te zijn dat de aankondiging ook daadwerkelijk naar al je volgende servers wordt gepushed, en zonder twijfel, ben je soms gewoon vergeten om op die knop te klikken!

Met Pepe Manager kunt u een aankondigingskanaal zo instellen dat alle aankondigingen die u naar het kanaal stuurt automatisch naar buiten worden gepusht! 

### Video-handleiding

Als u geen zin heeft om lang te lezen, hebben wij een video tutorial gemaakt die makkelijk te volgen moet zijn:

{% embed url="https://youtu.be/d6\_HNHrJ8lU" %}

## Handleiding

### Een aankondigingskanaal maken

De eerste stap om een aankondigingskanaal te maken is om de community server functies in te schakelen, door deze [gids](https://support.discord.com/hc/en-us/articles/360047132851-Enabling-Your-Community-Server) van Discord zelf te volgen!

De volgende stap is het aanmaken van een nieuw kanaal, en als kanaaltype te selecteren: 'Aankondigingskanaal'. Geef het een toepasselijke naam en ga dan door naar de volgende stap!

![](../.gitbook/assets/kzgyljb.png)

### Pepe Manager de juiste rechten geven

Deze volgende stap is vrij cruciaal. Standaard zal Pepe Manager geen berichten kunnen aankondigen in het nieuwe kanaal, en daarom moet je of Pepe Manager (De Bot Account) of Pepe Manager (De Integratie Role) de **Verstuur Berichten** permissie geven in het nieuw aangemaakte aankondigingskanaal.

{% hint style="info" %}
Maak je geen zorgen, de bot zal nooit zelf berichten naar je aankondigingskanaal sturen, hij heeft deze toestemming alleen nodig om berichten aan te kondigen die al verstuurd zijn.
{% endhint %}

![](../.gitbook/assets/ligkvrd.png)

### De automatische uitgever configureren

Tenslotte moeten we Pepe Manager vertellen welk aankondigingskanaal het automatisch moet publiceren! Standaard kunnen gratis servers tot 5 aparte automatische aankondigingskanalen instellen, maar [premium servers](../information/patreon-perks.md) kunnen tot 25 automatische aankondigingskanalen instellen. Om te beginnen, typt u het volgende commando:

Waar **&lt; &gt;** een verplichte parameter impliceert

```text
p!config set autoPublishChannels <Channel/ChannelID/ChannelMention>
```

### Final Words

En dat is het! U heeft met succes een automatisch publicerend aankondigingskanaal met Pepe Manager gemaakt!

Als u meer hulp nodig heeft met Pepe Manager, bekijk dan de rest van deze documentatie of sluit u aan bij onze support server om met een echt mens te praten!

