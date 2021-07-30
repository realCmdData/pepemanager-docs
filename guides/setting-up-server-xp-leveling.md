---
description: 'Beloon de activiteit van uw gebruikers met niveaus, rolbeloningen en meer!
---

# Set Up Server XP/Leveling

### Waarom zou je dit nodig hebben?

Server Leveling is een super gemakkelijke en effectieve manier om activiteit en groei in je Discord server te verzekeren. Door het uitzetten van doelen van activiteit met beloningen, zullen gebruikers worden verleid om de chat gaande te houden om dit doel te bereiken dat je voor hen hebt uitgezet. Dit doel kan van alles zijn, van iets simpels en goedkoop als een rol beloning die de gebruiker een speciale toestemming geeft, zoals de mogelijkheid om afbeeldingen te versturen en te embedden, tot het belonen van de meest actieve gebruikers op je Discord met Nitro!  
Pepe Manager biedt een gratis en makkelijk te gebruiken XP en Leveling systeem zodat je de gebruikers retentie hoog kunt houden, en de kosten laag!

### Video Handleiding

Als je een afkeer hebt van lang lezen, hebben we een video tutorial gemaakt die makkelijk te volgen is:

{% embed url="https://youtu.be/H-x3\_94-T8E" %}

## Handleiding

### Leveling inschakelen

Pepe Manager heeft standaard geen leveling ingeschakeld. Alle gebruikersactiviteiten die plaatsvonden voordat u leveling inschakelde, worden niet meegeteld. U moet het inschakelen om te beginnen door het volgende commando te typen:

```text
p!config toggle levels
```

### Toegestane kanalen toevoegen

Je kunt nu specifieke kanalen toevoegen waarin gebruikers XP kunnen verdienen. De kanalen die je instelt zullen de enige kanalen in de server zijn waar gebruikers XP kunnen verdienen. Je kunt meerdere kanalen toevoegen met hetzelfde commando \(door een spatie tussen de kanalen te plaatsen\) of je kunt ook een kanaal na elkaar toevoegen. Om kanalen toe te voegen kun je het volgende commando typen:

Waar **&lt; &gt;** een verplichte parameter inhoudt

```text
p!config set xpChannels <Channel/ChannelID/ChannelMention>
```

{% hint style="info" %}
Je kan het kanaal instellen door de naam van het kanaal te schrijven, het kanaal ID te gebruiken of door gewoon het kanaal te vermelden.  
Als je een onvolledige kanaalnaam schrijft zal de bot naar het dichtsbijzijnde kanaal zoeken.
{% endhint %}

{% hint style="success" %}
#### En dat is het!

Als je alleen de basis leveling setup wilt, ben je nu klaar! Als je meer de diepte in wilt gaan en over veel meer mogelijkheden wilt leren die je kunt gebruiken, ga dan verder!  
  
_**ALLE STAPPEN NA DIT PUNT ZIJN OPTIONEEL**_
{% endhint %}

### Geen XP Rollen toevoegen

Je kan nu instellen dat een bepaalde rol geen XP krijgt, ongeacht of de gebruiker in het juiste levelkanaal zit of niet. Het is ook niet belangrijk of de gebruiker een andere rol heeft boven of onder de rol die je instelt om geen XP te verdienen.   
Deze functie is erg handig als je niet wilt dat je personeel XP krijgt, of om ervoor te zorgen dat gedempte gebruikers geen XP krijgen, etc. Om een rol toe te voegen kun je het volgende commando typen:

Waar **&lt; &gt;** een verplichte parameter inhoudt

```text
p!config set noXpRoles <Role/RoleID/RoleMention>
```

{% hint style="info" %}
Je kan de rol instellen door de naam van de rol te schrijven, de rol ID te gebruiken of door de rol gewoon te vermelden.  
Als je een onvolledige rolnaam schrijft zal de bot zoeken naar de volgende dichtsbijzijnde, dit is handig als je systeem emoji's hebt als onderdeel van je rolnaam.
{% endhint %}

### De Top XP rol toevoegen

Je kan een gebruiker met de meeste XP ook belonen door de bot een Top XP rol toe te laten kennen. Deze rol wordt gegeven om 00:00 UTC, en wordt maar aan één persoon gegeven op de server. Als een gebruiker eerder de Top XP rol had, zal het van hem worden afgenomen.   
Deze functie is een snelle en makkelijke manier om gebruikers een lange termijn doel te geven om naar toe te werken. Het helpt ook als de Top XP rol vrij hoog op de serverlijst staat, en een prominente kleur krijgt. Om de Top XP rol in te stellen, kun je het volgende commando typen:

Waar **&lt; &gt;** een verplichte parameter inhoudt

```text
p!config set topXpRole <Role/RoleID/RoleMention>
```

{% hint style="warning" %}
Het is **zeer** aan te raden om de Top XP rol ook in te stellen als een No XP rol. Als je dit niet doet kan het gebeuren dat maar één persoon ooit de Top XP rol krijgt omdat hij tijdens zijn dag aan de Top XP blijft verdienen.  
Door ze een dag geen XP te laten verdienen krijgen andere gebruikers de tijd om in te halen.
{% endhint %}

### Level-Op Bericht Aanpassen

Als u vindt dat het huidige Level-Up bericht niet bij uw serverstijl past, of u wilt het gewoon wat pittiger maken, dan kunt u het volledig aanpassen! Wij ondersteunen momenteel alleen ruwe tekstberichten \(niet Embeds\)  
Om het Level-Up bericht in te stellen kun je het volgende commando typen:

Waar **&lt; &gt;** een verplichte parameter inhoudt

```text
p!config set xpMessage <Message>
```

Er zijn verschillende **tags** die je in je Level-Up bericht kunt opnemen. Deze parameters zullen worden vervangen door de juiste informatie wanneer het Level-Up bericht wordt verzonden.  
  
_Je moet de {} haakjes in je bericht opnemen om de tags te laten verschijnen!_

| Information | Parameter |
| :--- | :--- |
| Gebruiker Vermelding \(@User\) | {user} |
| Gebruiker Tag \(User\#1234\) | {user.tag} |
| Gebruikersnaam \(User\) | {user.username\) |
| Gebruikersdiscriminator \(1234\) | {user.discriminator} |
| Gebruikers-ID \(99787644430475264\) | {user.id} |
| Server Naam \(My Cool Server\) | {guild.name} |
| Server-ID \(493351982887862283\) | {guild.id} |
| Level Bereikt \(5\) | {level} |

### Waar het Level-Up bericht te verzenden

Standaard zal Pepe Manager het Level-Up bericht in hetzelfde kanaal sturen als waar de gebruiker die het laatst met een Level-Up heeft gesproken, maar dit kan soms opdringerig zijn en kan een normaal gesprek verstoren. Maak je echter geen zorgen, want je kunt instellen waar Pepe Manager het Level-Up bericht naartoe zal sturen. Om dit in te stellen, type je simpelweg het volgende commando:

Waar **&lt; &gt;** een verplichte parameter inhoudt

```text
p!config set xpResponseType <Type>
```

Er zijn verschillende reactietypes waaruit u kunt kiezen. U kunt er slechts één tegelijk kiezen, en het Level-Up bericht dat u eventueel eerder hebt ingesteld, zal naar elk reactietype worden overgedragen. 

| Waar wordt het heen gestuurd? | Typ antwoord |
| :--- | :--- |
| In hetzelfde kanaal als de gebruiker | channel |
| In de directe berichten van de gebruiker | dm |
| De hele tijd in een specifiek kanaal | \#Channel |
| Nergens. Alle berichten zijn uit | off |

### Rolbeloningen toevoegen

De hoofdmoot van het Leveling: de rolbeloningen. Je kunt rollen instellen die aan gebruikers worden gegeven als ze een bepaald niveau bereiken. Dit kan gebruikt worden om het level van een gebruiker aan te duiden met een rol, speciale kleuren aan gebruikers te geven als ze een hoger level bereiken, permissies te geven die verdiend kunnen worden door activiteit, en nog veel meer.   
Met de gratis versie van Pepe Manager kunt u tot 2 rollen instellen om te worden gegeven op hetzelfde niveau, maar over het algemeen is er geen limiet aan het aantal rollen dat u kunt instellen.  
De premium limiet is 10 rollen voor hetzelfde niveau.

Waar **&lt; &gt;** een verplichte parameter inhoudt

```text
p!config set xpRoles <Level> <Role/RoleID/RoleMention>
```

{% hint style="info" %}
Let op: als je rol meerdere woorden bevat, zoals de rol **Cool Persoon**, moet je ofwel de Rol ID of Vermelding gebruiken, of alleen het woord **Cool** schrijven.  
  
De bot zal de woorden **Cool** en **Persoon** als aparte rollen zien.
{% endhint %}

### Levels automatisch resetten

Het automatisch resetten van levels kan zeer nuttig zijn om uw server mooi en georganiseerd te houden, en om diegenen die u verbant nog meer te straffen!  
Wanneer aan de door u ingestelde voorwaarde is voldaan, zal Pepe Manager automatisch de levelgegevens van de betreffende gebruiker (als ze die hadden) resetten zonder vragen te stellen. **Het schoppen van een gebruiker heeft hetzelfde effect als weggaan, dus wees voorzichtig!**

Waar **&lt; &gt;** een verplichte parameter inhoudt

```text
p!config set autoResetLevels <Type>
```

Er zijn verschillende soorten reacties waaruit u kunt kiezen. U kunt er maar één tegelijk kiezen.

| Wat zal de reset teweegbrengen? | Typ antwoord |
| :--- | :--- |
| Niets | none |
| Wanneer de gebruiker de server verlaat om wat voor reden dan ook | leave |
| Wanneer de gebruiker is verbannen om welke reden dan ook | ban |
| Wanneer de gebruiker vertrekt of wanneer de gebruiker wordt verbannen | both |

### Rol stapelen

Nu je enkele rolbeloningen hebt ingesteld, kan je kiezen of de bot de rollen al dan niet zal stapelen. Stapelen betekent dat elke extra rolbeloning gewoon toegevoegd zal worden aan de reeds bestaande rollen van de gebruiker. Niet stapelen betekent dat alle vorige rolbeloningen verwijderd zullen worden wanneer de gebruiker een nieuwe rol krijgt. Dit heeft geen invloed op rollen die niet specifiek gemarkeerd zijn als beloning.  
Standaard staat stapelen **aan**.

```text
p!config toggle stackXpRoles
```

### Laatse woorden

Het is heel eenvoudig om een activity tracking systeem op te zetten, maar als u meer en meer functies wilt toevoegen, en uw gebruikers wilt belonen voor hun loyaliteit en acitviteit wordt het steeds complexer. Als je nieuw bent met bots, wees dan niet bang voor alle ingewikkelde commando's en commandostructuren, nieuwe woorden die bots gebruiken om te beschrijven wat ze doen, enz.  
Bots kunnen een fantastisch hulpmiddel zijn om een geweldige gemeenschap op te bouwen, en het leren van de innerlijke werking van een bot waar je toch al veel tijd mee gaat doorbrengen kan later van pas komen.

