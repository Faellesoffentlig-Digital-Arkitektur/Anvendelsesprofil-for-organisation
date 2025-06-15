# Bilag A -- Baggrund for basisprofil for organisation {#bilag-a-baggrund-for-basisprofil-for-organisation}

## Profilens udgangspunkt og tilblivelse

Denne anvendelsesprofil er det foreløbige resultat af forslaget
*Fællesoffentlig standard for Organisation*, der blev vedtaget af
'Udvalget for arkitektur og standarder' (UAS) på 6. møde 8 juni 2021.
Forslagets hovedindhold var:

#### *Forslag*

*Initiativet har til formål at gøre det lettere at udveksle
organisationsoplysninger mellem myndigheder og på tværs af sektorer. Det
skal ske ved at skabe én fælles forståelse af hvad organisation er og
hvilke informationer der beskriver en organisation. Der tages afsæt i
aktuelle behov og eksisterende erfaringer med forskellige standarder for
at beskrive organisationer på tværs af sektorer.*

#### *Baggrund*

*Organisationsoplysninger er en fast bestanddel af de offentlige
it-løsninger. Oplysninger er særlige relevante når rettigheder skal
håndteres, data skal kommunikeres og handlinger skal dokumenteres.
Organisation dækker over flere forskellige aspekter som fx
organisationens hierarkiske struktur, kontaktoplysninger, ansvar,
roller, opgaver m.fl. Det vil være op til de forskellige
anvendelsesscenarier at afgøre hvilke aspekter der er nødvendige.*

*Der anvendes flere forskellige måder at beskrive organisationer på
tværs i det offentlige i dag. På sundhedsområdet er det standarden SOR
der er bredt anvendt, i kommunerne er det OIO Organisation og i
projekter under FODS har FDA-profilen været anvendt.*

*Manglen på fælles sprog om de offentlige organisationer udfordrer
kvaliteten i de tværgående processer mellem myndigheder og har bl.a.
afledte udfordringer i forhold til at adressere de korrekte medarbejdere
på tværs af myndigheder samt i forhold til at håndtere sikkerhedsmæssige
aspekter som fx at håndhæve rettigheder i fælles it-løsninger.
Udfordringerne er anerkendt på tværs af såvel stat, regioner og
kommuner - handling efterspørges af alle parter.*

*Initiativet skal derfor afdække centrale anvendelsesmæssige behov på
tværs af stat, kommuner, regioner med udgangspunkt i erfaringer med
førnævnte standarder. Behovsafdækningen skal lede til etablering af en
fællesoffentlig standard til at beskrive organisationer - standarden
udarbejdes efter retningslinjerne i de fællesoffentlige regler for
modellering (FDA modelregler). For at sikre sammenhæng til eksisterende-
og kommende EU-standardisering, kan en fællesoffentlig standard evt.
tage afsæt i den eksisterende FDA-profil for Organisation (baseret på
internationale standarder).*

*Fokus i initiativet er på at frembringe en MVP (Minimum Viable Product)
som sikrer at centrale dele af oplysninger om organisationer kan deles
mellem myndigheder. MVP'en kan derefter videreudvikles med fx profiler
til at understøtte særlige use cases, fastlæggelse af klassifikationer
og/eller etablering af en egentlig referencearkitektur for
organisation.*

#### *Strategisk ophæng*

*Initiativet understøtter såvel den overordnede vision om en
sammenhængene offentlig sektor, samt flere hovedprincipper fra Hvidbogen
om Fællesoffentlig digital arkitektur. Et fælles sprog om organisationer
vil højne sammenhængen i den offentlige sektor ved at lette deling og
anvendelse af efterspurgte grundlæggende informationer. Et fælles sprog
vil ligeledes understøtte målet om at kommunikere effektivt samt
understøtte en sikker håndtering af adgang til fortrolige data.*

*Det har været længe været en ambition at have en fællesoffentlig
standard for Organisation.*

Med udgangspunkt i det vedtagne forslag blev der dannet en
referencegruppe med henblik på at få afdækket centrale
anvendelsesmæssige behov på tværs af stat, kommuner, regioner.

Behovsafdækningen resulterede i dokumentet *Brugerbehov til
Fællesoffentlig standard for Organisation*
[^[1]{.underline}^](https://github.com/digst/Basisanvendelsesprofil-for-organisation/blob/main/Basisanvendelsesprofil/2)%20Profilens%20udgangspunkt%20og%20tilblivelse.md#user-content-fn-1-3db06bca7ff73be10a1f53a4c49459ab).

Ud fra brugerbehovene blev der udformet en begrebsmodel som en
informationsmodel for organisation. Informationsmodellen startede med at
favne stort set alle registrerede behov i en relativt omfattende model,
men endte med at fokusere på de centrale elementer for en
organisationsmodel. Det er denne seneste model, *FOOM - kernemodel for
organisation*, der har dannet grundlag for udformningen af nærværende
anvendelsesprofil. ('FOOM' står her for '**F**ælles**o**ffentlig
**O**rganisations**m**odel'.)

### Tidligere forslag til anvendelsesprofil

I det forslag UAS vedtog står:

> "For at sikre sammenhæng til eksisterende- og kommende
> EU-standardisering, kan en fællesoffentlig standard evt. tage afsæt i
> den eksisterende FDA-profil for Organisation (baseret på
> internationale standarder)."

Den FDA-profil der henvises til var et tidligere udkast til
anvendelsesprofi, baseret på *The Organization Ontology* [^1] (ORG) og
*Core Public Organisation Vocabulary* [^2] (CPOV). I den nuværende
første udgave af basisprofilen er ORG stadig en væsentlig kilde til
elementer der indgår i profilen, mens der aktuelt kun er medtaget et
enkelt element (adms:Identifier) (fra CPOV.

Det tidligere forslag kan ses her:
<https://arkitektur.digst.dk/specifikationer/organisation/anvendelsesprofil-organisationer>

I processen er der gjort brug af modellerne for henholdsvis
*Fælleskommunalt Organisationssystem* (FK-ORG) og *Sundhedsvæsenets
Organisationsregister* (SOR) som referencepunkter inden for de rammer
der blev sat af informationsmodellen FOOM.

[^1]: <https://www.w3.org/TR/vocab-org/>

[^2]: <https://semiceu.github.io/CPOV/releases/2.1.0/>
