---
description: >-
  Leer hoe Pepe Manager automatisch nieuwe gebruikers rollen kan toewijzen zonder
  het Discord verificatie systeem te breken!
---

# Automatisch toevoegen van rollen \(met time-out\)

### Waarom zou je dit nodig hebben?

Automatisch rollen toevoegen aan nieuwe leden kan vele nuttige doelen dienen, van het geven van een coole kleur aan nieuwe leden in je chat, tot het geven van toestemmingsrollen die kunnen worden weggehaald indien nodig, of voor het toevoegen van ping rollen voor aankondigingen.  
Echter, als je een Discord verificatieniveau hebt ingeschakeld dat gebruikers die het verificatieniveau niet overschrijden nodig maakt, zal het automatisch toevoegen van een rol wanneer iemand toetreedt deze verificatiefilter omzeilen! Pepe Manager staat je toe om een timer in te stellen vanaf het moment dat een gebruiker toetreedt tot wanneer hij de rol zal ontvangen, zodat het verificatie systeem niet omzeild wordt!

### Video-handleiding

Als u geen zin hebt om lang te lezen, hebben wij een video gemaakt die u gemakkelijk zou moeten kunnen volgen:

{% embed url="https://youtu.be/94NleboBP\_o" %}

## Handleiding

### Uw verificatieniveau evalueren

Om deze handleiding zo effectief mogelijk te laten zijn, moet je naar je serverinstellingen gaan, naar het tabblad Moderatie, en dubbel-checken welk verificatieniveau je hebt geselecteerd.

![](https://i.imgur.com/dZ9o0ae.png)

Het verificatieniveau **Medium** heeft een time-out van 5 minuten, terwijl de instellingen **Hoog** en **Hoogst** een time-out van 10 minuten hebben.

### Uw Autorollen instellen

U kunt nu uw autorollen toevoegen aan Pepe Manager. In de huidige versie is het niet mogelijk om verschillende rollen aan verschillende time-outs toe te wijzen, ze zullen allemaal tegelijkertijd worden toegewezen.  
De gratis versie van de bot staat u toe om tot 5 autorollen tegelijkertijd toe te wijzen, terwijl de premium versie u toestaat om tot 25 autorollen toe te wijzen. [Klik hier voor meer informatie](../information/patreon-perks.md).

Waar **&lt; &gt;** een verplichte parameter inhoudt

```text
p!config set autoRole <Role/RoleID/RoleMention>
```

{% hint style="warning" %}
Je kunt al je autorollen met hetzelfde commando instellen door een spatie tussen elke rol te zetten, dit werkt echter alleen voor Rol Vermeldingen en Rol ID's, als één of meer van de rollen die je wilt toewijzen een spatie in hun naam hebben.  
Spaties worden behandeld als scheidingstekens, en als je de volledige rolnaam met een spatie invoert, zal Pepe Manager ze behandelen als 2 aparte rollen.
{% endhint %}

### Time-out instellen

Je kunt nu instellen hoelang de bot moet wachten met het toewijzen van de rollen nadat een gebruiker zich heeft aangemeld. Dit is niet beperkt tot 5 minuten of 10 minuten, je kunt de timeout instellen op 1 minuut of zelfs 30 minuten.

Waar **&lt; &gt;** een verplichte parameter inhoudt

```text
p!config set autoRoleTimeout <Time>
```

### Laatste woorden

En dat is het! U heeft met succes Automatisch Rollen Toekennen met Pepe Manager gemaakt!

Als u meer hulp nodig heeft met Pepe Manager, bekijk dan de rest van deze documentatie of sluit u aan bij onze support server om met een echt mens te praten!

