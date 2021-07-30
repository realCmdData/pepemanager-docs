---
description: Ontdek hoe Pepe Manager automatisch een mijlpaal met u kan vieren!
---

# Automatisch gecontroleerde mijlpalen voor leden

### Waarom zou u dit nodig hebben?

Het vieren van een mijlpaal van een lid is een super eenvoudige en sociale activiteit. Of u nu 100 leden viert of 100.000, het is net zo'n gedenkwaardige gebeurtenis als elke andere. Door het vieren en belonen van de gebruiker die lid werd als uw n-de lid, kunt u altijd een nieuw doel te bereiken, een nieuw niveau van groei te bereiken. Het automatiseren van dit proces is snel en eenvoudig, en de mogelijkheden zijn eindeloos!

### Video Handleiding

Als u geen zin heeft om lang te lezen, hebben wij een video tutorial gemaakt die u gemakkelijk kunt volgen:

{% embed url="https://youtu.be/nXlhdcH3YaU" %}



## Handleiding

### Mijlpalen inschakelen

De eerste stap is het inschakelen van de mijlpaalfunctie in uw Pepe Manager-instellingen. Dit werkt als een handige schakelaar als u wilt stoppen met het gebruik van mijlpalen, maar al uw geconfigureerde instellingen wilt behouden waar we later op in zullen gaan. Om het in te schakelen, type het volgende commando:

```text
p!config toggle milestones
```

### Het mijlpaalkanaal instellen

De volgende stap is het instellen van een mijlpaal kanaal, waar al uw geautomatiseerde mijlpaal aankondigingen in zullen worden verzonden! Dit kan een gewoon tekstkanaal zijn of als u een community enable server heeft, kan dit ook een aankondigingskanaal zijn. Om uw kanaal in te stellen, type het volgende commando:

Waar **&lt; &gt;** een verplichte parameter inhoudt

```text
p!config set milestonesChannel <Channel/ChannelID/ChannelMention>
```

### Het mijlpaalinterval instellen

Deze volgende stap is heel belangrijk omdat u nu kunt kiezen bij hoeveel leden u de mijlpaal wilt laten afgaan. Het interval is het aantal leden tussen elke mijlpaal, en standaard is het ingesteld op **100**. Dit betekent dat elke 100 leden een mijlpaal wordt getriggerd, zoals **200**, **300**, **400**, enz.  
Het mijlpaalinterval kan elk willekeurig getal zijn, zolang het maar een _**veelvoud van 5**_ is. Zo kan het interval worden ingesteld op **5** of op **100.000**. Om uw interval in te stellen, typt u het volgende commando:

Waar **&lt; &gt;** een verplichte parameter inhoudt

```text
p!config set milestonesInterval <Number>
```

### Het mijlpaalbericht instellen

Vervolgens kunt u ook uw mijlpaalbericht aanpassen, dat is het bericht dat wordt verstuurd wanneer een mijlpaal is bereikt. Standaard ziet het bericht er als volgt uit:

![](https://i.imgur.com/IUZMJGP.png)

U kunt een willekeurig aantal emoji's \(zolang de bot ze kan openen\), opmaak, regeleinden, speciale tekens en zelfs rolvermeldingen toevoegen, zolang het binnen de 2000 karakterlimiet van alle berichten blijft. Om je mijlpaal bericht in te stellen, type het volgende commando:

Waar **&lt; &gt;** een verplichte parameter inhoudt

```text
p!config set milestonesMessage <Message>
```

{% hint style="warning" %}
Als u een rolvermelding in uw bericht opneemt, zorg er dan voor dat Pepe Manager toestemming heeft om die rol te vermelden, anders zal het niet werken en kan het bericht er erg lelijk uitzien.
{% endhint %}

Er zijn verschillende **tags** die u in uw Mijlpaal-bericht kunt opnemen. Deze parameters worden vervangen door de juiste informatie wanneer het Mijlpaalbericht wordt verzonden.  
  
_U moet de {} haakjes in uw bericht opnemen om de tags te kunnen weergeven!_

| Informatie | Tag |
| :--- | :--- |
| Gebruiker Vermelding \(@User\) | {user} |
| Gebruiker Tag \(User\#1234\) | {user.tag} |
| Gebruikersnaam \(User\) | {user.username\) |
| Gebruikersdiscriminator \(1234\) | {user.discriminator} |
| Gebruikers-ID \(99787644430475264\) | {user.id} |
| Server Naam \(My Cool Server\) | {guild.name} |
| Server-ID \(493351982887862283\) | {guild.id} |
| Mijlpaal Bereikt \(100\) | {milestone} |

### De rol van mijlpalen instellen

Tenslotte kunt u ook gebruikers belonen die op het juiste moment lid zijn geworden door hen een rol of meerdere rollen toe te kennen. Gratis servers kunnen tot **5** rollen toekennen aan die speciale persoon, en [Premium](../information/patreon-perks.md)-servers kunnen tot **10** rollen toekennen. Om je mijlpaal rol\(len\) in te stellen, type het volgende commando:

Waar **&lt; &gt;** een verplichte parameter inhoudt

```text
p!config set milestonesRole <Role/RoleID/RoleMention>
```

### Final Words

En dat is het! U heeft met succes Automatisch Rollen Toekennen met Pepe Manager gemaakt!

Als u meer hulp nodig heeft met Pepe Manager, bekijk dan de rest van deze documentatie of sluit u aan bij onze support server om met een echt mens te praten!

