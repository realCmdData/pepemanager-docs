# Sjekk

### Beskrivelse

{% hint style="warning" %}
Dette er en **Metode** eller en **underkommando** av [Config ](./)command. Det er ikke sin egen kommando.
{% endhint %}

Denne metoden av [config ](./)command kan bli brukt til å sjekke om du har lagt inn alle konfigurasjonsnøklene riktig. Kommandoen vil svare med et innebygging som inneholder nøkkelnavnet og verdien det er satt til.

Hvis en nøkkel ikke er angitt, viser den en 'No Sign' emoji.  
Hvis en **set** nøkkel er riktig konfigurert, viser den hva verdien er satt til.  
Noen **sett** -taster er konfigurert til en standardverdi, som også vil bli vist på kontrollkommandoen.
Hvis en **veksle** -tast er satt til true, vil den vise en "Yes Sign" -emoji, og hvis den er satt til falsk, vil den vise en "No Sign" -emoji.

### Kommandostruktur

```text
p!config check
```

Nedenfor er en tabell som inneholder alle konfigurasjonsnøkler som vises i kontrollmetoden, sammen med alle standardverdiene.

| Nøkkel | Standard Sjekkverdi |
| :--- | :--- |
| Milestones Kanal | ❌ \(Ikke Satt\) |
| Milestone Intervall | ✅ \(100\) |
| Prefix | ✅ \(p!\) |
| Medlemstall  | ✅ \(På\) |
| Automatisk Rolle | ❌ \(Ikke Satt\) |
| Automatisk Rolle Pause | ❌ \(Ikke Satt\) |
| Emoji Liste | ❌ \(Ikke Satt\) |
| Blokkerte Kanaler | ❌ \(Ikke Satt\) |
| XP Kanaler | ❌ \(Ikke Satt\) |
| XP Roller | ❌ \(Ikke Satt\) |
| Stable XP Roller | ✅ \(Sant\) |
| Topp XP Rolle | ❌ \(Ikke Satt\) |
| Ingen XP Roller | ❌ \(Ikke Satt\) |
| Automatisk Publisering av Kanaler | ❌ \(Ikke Satt\) |
| Rolle Nevning Nedkjøling | ✅ \(0ms\) |
| Nevn Roller Nedkjølin | ❌ \(Ikke Satt\) |
| XP Respons type | ✅ \(Samme kanal\) |
| XP Melding | ✅ \({user} has reached level **{level}**\) |
| Milestone Melding | ✅ \(**{milestone} Members**  Congratulations to {user}, you were the {milestone}th person to join!\) |

### **Tillatelse**

* `Administrer server`**\(Bruker\)**
* N/A **\(Bot\)**

### Aliaser

* N/A



