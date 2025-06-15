# Om profilen

Basisprofilen for organisation er en anvendelsesprofil med fokus på
organisationer og organisatoriske forhold. Profilens formål er at gøre
udveksling af organisationsdata mellem it-systemer mere præcis og
entydig ved at anvende entydige metadata og struktur til beskrivelse af
udvekslede data. Ved at anvende basisprofilen til at beskrive delte data
gøres det både lettere at anvende modtagne data og kvalitet i tolkning
af data sikres bedst muligt mod misforståelser.

Den fællesoffentlige organisationsmodel er udformet som en basisprofil
der kan inddrages efter behov af it-systemer der ønsker at indgå i et
semantisk interoperabelt fællesoffentligt landskab.

Basisprofil for organisation vil på den måde blive en semantisk
byggeblok der kan bygges videre på af de anvendende systemer. Der vil
eksempelvis for FK-ORG og SOR kunne defineres API-profiler hvor de
centrale elementer genbruges direkte fra basisprofilen, mens de mere
systemspecifikke elementer tilføjes API-profilen.

Basisprofilen er ikke tænkt som en statisk størrelse. Profilen vil kunne
ændres, vi kunne få tilføjes nye elementer i hele profilens levetid. Den
primære kilde til fornyelse vil komme fra de API-profiler der benyttes
basisprofilen. Hvis det vurderes at to eller flere API-profiler har et
sammenfald i funktion OG hvis den funktion vurderes at ville give
basisprofilen øget værdi, så fornys basisprofilen.

I 'Bilag A - Anvendelsesprofiler for semantisk interoperabilitet',
udfoldes begreberne 'Basisprofil' og 'API-profil'. Det anbefales at læse
bilaget.

Information vedrørende baggrunden for profilens oprettelse kan findes i
'Bilag B -- Baggrund for basisprofil for organisation'.

### Grunddatamodel

I arbejdet med basisprofilen har der været opmærksomhed på at inkludere
eksplicitte referencer til grunddatamodellerne, hvor det har været
relevant og muligt.

I nuværende udgave er dette begrænset til en enkelt reference (DAR-ID),
men der ses et potentiale i kombinationen af basisprofiler generelt og
API-profiler for grunddata.

### Redaktionsgruppe og det videre arbejde

Som nævnt tidligere, så vil det være muligt at ændre, udvide og
kvalificere basisprofilen efterfølgende. Dette gælder både den egentlige
profil og de relaterede klassifikationer og vokabularer. For at sikre at
nye versioner frembringes så hurtigt og sikkert som muligt, så bør
basisprofilen tilknyttes til en redaktionsgruppe der blandt andet skal
varetage spørgsmål som ovenstående.

## Metode

Anvendelsesprofilen er oprettet i henhold de [Fællesoffentlige regler
for begrebs- og
datamodellering](https://arkitektur.digst.dk/metoder/regler-begrebs-og-datamodellering),
og sammensætter således eksisterende vokabularer til en bestemt
anvendelse. Teknologisk udspringer de anvendte og foreslåede modeller af
Semantic Web/Linked Data-verdenens modelleringsgrundlag, Resource
Description Framework (RDF). En basal forståelse af RDF samt kendskab
til de her profilerede vokabularer er et godt udgangspunkt for arbejdet
med anvendelsesprofilen. For en kort introduktion til RDF kan man med
fordel læse den oversatte RDF 1.1 Primer :
<https://data.gov.dk/W3C/rdf-primer-danish.html>

## Anvendte vokabularer

I profilen er der anvendt et udvalg af vokabularer.

For at lette læsbarheden i dokumentet, angives URIer i deres kompakte
form hvor det er muligt. I en kompakt form er navnerum erstattet af et
præfiks, eksempelvis som illustreret her:

> Hvis navnerummet: http://www.w3.org/ns/org#
> 
> tildeles præfiks: org
> 
> så kan URIen: http://www.w3.org/ns/org#OrganizationalUnit
> 
> angives i kompakt form som: org:OrganizationalUnit

Præfiks og navnerum for de anvendte vokabularer er listet herunder.

| **præfiks** | **navnerum**                                                                                | **titel**                            |
| ----------- | ------------------------------------------------------------------------------------------- | ------------------------------------ |
| rdf         | [http://www.w3.org/1999/02/22-rdf-syntax-ns#]{.underline}                                   | Resource Description Framework       |
| rdfs        | [[http://www.w3.org/2000/01/rdf-schema#]{.underline}](http://www.w3.org/2000/01/rdf-schema) | RDF Schema                           |
| owl         | [[http://www.w3.org/2002/07/owl#]{.underline}](http://www.w3.org/2002/07/owl)               | Web Ontology Language                |
| xsd         | [[http://www.w3.org/2001/XMLSchema#]{.underline}](http://www.w3.org/2001/XMLSchema)         | XML Schema                           |
| skos        | [[http://www.w3.org/2004/02/skos/core#]{.underline}](http://www.w3.org/2004/02/skos/core)   | Simple Knowledge Organization System |
| org         | [[http://www.w3.org/ns/org#]{.underline}](http://www.w3.org/ns/org)                         | Organization Ontology                |
| foaf        | [[http://xmlns.com/foaf/0.1/]{.underline}](http://xmlns.com/foaf/0.1/)                      | Friend of a Friend                   |
| dcterms     | [[http://purl.org/dc/terms/]{.underline}](http://purl.org/dc/terms/)                        | Dublin Core Metadata Terms           |
| schema      | [[http://schema.org/]{.underline}](http://schema.org/)                                      | Schema.org                           |
| adms        | [[http://www.w3.org/ns/adms#]{.underline}](http://www.w3.org/ns/adms)                       | ADMS Vocabulary                      |
| prov        | [http://www.w3.org/ns/prov#](http://www.w3.org/ns/prov)                                     | PROV-O: The PROV Ontology            |

### Vokabular oprettet i relation til arbejdet med profilen

Arbejdet med basisprofilen gav anledning til oprettelse af en række
supplerende vokabularer og klassifikationer. Disse vil naturligvis kunne
anvendes i andre sammenhænge end den de her er anvendt i.

De nyoprettede er:

| **præfiks** | **navnerum**                                             | **titel**                         |
| ----------- | -------------------------------------------------------- | --------------------------------- |
| ovx         | https://data.gov.dk/model/core/orgextension/             | Organization vocabulary extension |
| fot         | https://data.gov.dk/concept/core/formalorganizationtype/ | Formal organization type          |
| out         | https://data.gov.dk/concept/core/organisationalunittype/ | Organizational unit type          |
| ci          | https://data.gov.dk/concept/core/contactinformation/     | Contact information               |
| ort         | https://data.gov.dk/concept/core/orgrelation/            | Organizational Relation           |

##### Footnotes

1. [[https://github.com/digst/ORG-AP-DK/blob/main/releases/v.1.0/business/Brugerbehov%20til%20F%C3%A6llesoffentlig%20standard%20for%20Organisation%20%E2%80%93%202022-02-18_KL20221014.docx]{.underline}](https://github.com/digst/ORG-AP-DK/blob/main/releases/v.1.0/business/Brugerbehov%20til%20F%C3%A6llesoffentlig%20standard%20for%20Organisation%20%E2%80%93%202022-02-18_KL20221014.docx)
   [[↩]{.underline}](https://github.com/digst/Basisanvendelsesprofil-for-organisation/blob/main/Basisanvendelsesprofil/2)%20Profilens%20udgangspunkt%20og%20tilblivelse.md#user-content-fnref-1-3db06bca7ff73be10a1f53a4c49459ab)

2. [[https://github.com/digst/ORG-AP-DK/blob/main/releases/v.1.0/business/FOOM%20-%20f%C3%A6llesoffentligOrganisationsmodel%20v07.docx]{.underline}](https://github.com/digst/ORG-AP-DK/blob/main/releases/v.1.0/business/FOOM%20-%20f%C3%A6llesoffentligOrganisationsmodel%20v07.docx)
   [[↩]{.underline}](https://github.com/digst/Basisanvendelsesprofil-for-organisation/blob/main/Basisanvendelsesprofil/2)%20Profilens%20udgangspunkt%20og%20tilblivelse.md#user-content-fnref-2-3db06bca7ff73be10a1f53a4c49459ab)

3. [[https://www.w3.org/TR/vocab-org/]{.underline}](https://www.w3.org/TR/vocab-org/)
   [[↩]{.underline}](https://github.com/digst/Basisanvendelsesprofil-for-organisation/blob/main/Basisanvendelsesprofil/2)%20Profilens%20udgangspunkt%20og%20tilblivelse.md#user-content-fnref-3-3db06bca7ff73be10a1f53a4c49459ab)

4. [[https://semiceu.github.io/CPOV/releases/2.00/]{.underline}](https://semiceu.github.io/CPOV/releases/2.00/)
   [[↩]{.underline}](https://github.com/digst/Basisanvendelsesprofil-for-organisation/blob/main/Basisanvendelsesprofil/2)%20Profilens%20udgangspunkt%20og%20tilblivelse.md#user-content-fnref-4-3db06bca7ff73be10a1f53a4c49459ab)

5. [[https://semiceu.github.io/Core-Location-Vocabulary/releases/2.00/]{.underline}](https://semiceu.github.io/Core-Location-Vocabulary/releases/2.00/)
   [[↩]{.underline}](https://github.com/digst/Basisanvendelsesprofil-for-organisation/blob/main/Basisanvendelsesprofil/2)%20Profilens%20udgangspunkt%20og%20tilblivelse.md#user-content-fnref-5-3db06bca7ff73be10a1f53a4c49459ab)

6. [[https://semiceu.github.io/ADMS/releases/2.00/]{.underline}](https://semiceu.github.io/ADMS/releases/2.00/)
   [[↩]{.underline}](https://github.com/digst/Basisanvendelsesprofil-for-organisation/blob/main/Basisanvendelsesprofil/2)%20Profilens%20udgangspunkt%20og%20tilblivelse.md#user-content-fnref-6-3db06bca7ff73be10a1f53a4c49459ab)

## Beskrivelse af anvendte vokabularelementer

I et forsøg på at dokumentere anvendelsesprofilen bedst muligt, med
størst mulig transparens, er profilens elementer beskrevet med en
opdeling i henholdsvis det oprindelige vokabulars metadata samt
profilens metadata.

Konkret er elementbeskrivelserne opdelt som:

- Vokabularets definition og beskrivelser

- Profilens restriktioner og beskrivelser

Eksempelvis som vist her:

![](media/image1.png){width="5.708333333333333in"
height="3.5034722222222223in"}

Når et element fra et vokabular anvendes så er det samtidigt en accept
af de definitioner og beskrivelser vokabularet har givet. I profilen kan
elementet tilføjes restriktioner -- eksempelvis i udfaldsrum -- og/eller
yderligere beskrivelser, begge dele som en tilpasning til brug inden for
profilens rammer. Hverken restriktioner eller beskrivelser, tilføjet
under profilen, må stride imod vokabularets oprindelige definitioner og
beskrivelser.

Eksempelvis har elementet 'kontaktpunkt' (vist ovenfor) følgende domæne
fra vokabularet schema.org:

![](media/image2.png){width="5.708333333333333in"
height="0.400090769903762in"}

I profilen er dette gjort mere specifikt ved:

![](media/image2.png){width="5.708333333333333in"
height="0.26093941382327207in"}

Profilens indsnævring af domæner til kun at være org:FormalOrganization
eller org:OganizationalUnit er indenfor rammerne af vokabularets
definition. Ifølge beskrivelserne i schema.org kan schema:Organization
bruges både til at beskrive en formel organisation og en organisatorisk
enhed.

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>schema.org’s brug af ‘Domæne inkluderer’ + ‘Udfaldsrum
inkluderer’</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Vokabularet schema.org bruger deres egne egenskaber
schema:domainIncludes og schema:rangeIncludes i stedet for de normalt
benyttede rdfs:domain og rdfs:range.</p>
<p>Vokabularet beskriver dem således:</p>
<blockquote>
<p>domainIncludes</p>
<p>Relaterer en egenskab til en klasse, der er (en af) den eller de
typer egenskaben forventes at blive brugt på</p>
<p>rangeIncludes</p>
<p>Relaterer en egenskab til en klasse, der udgør (en af) de forventede
type(r) for værdier af egenskaben.</p>
</blockquote>
<p>Når der til egenskaberne er angivet flere klasser kan disse tolkes
som en foreningsmængde.</p>
<p>Anvendelsesprofilen bruger de to egenskaber på den måde de er
defineret i schema.org’s eksperimenterende OWL-udgave, <a
href="https://schema.org/docs/schemaorg.owl">schemaorg.owl</a> , hvor
rdfs:domain og rdfs:range benyttes i stedet for de to schema.org
egenskaber.</p></td>
</tr>
</tbody>
</table>

### Definitioner og beskrivelser

Alle klasser og alle egenskaber har en række metadata fælles. I
nedenstående tabel vises hvilke for henholdsvis vokabular- og
profil-beskrivelser.

Et felt markeret med gråt viser at metadata-egenskaben ikke har en egen
værdi i den pågældende sammenhæng. Specifikt gælder det at et elements
URI kun defineres i det vokabular der definerer elementet, samt at
multiplicitet for en egenskab kun defineres i profiler.

|                                     | **Vokabular**       | **Profil** |
| ----------------------------------- | ------------------- | ---------- |
| URI                                 | Skal altid udfyldes |            |
| Term (= rdfs:label)                 |                     |            |
| Foretrukken term (= skos:prefLabel) |                     |            |
| Alternativ term (= skos:altLabel)   |                     |            |
| Definition (= skos:definition)      |                     |            |
| Beskrivelse (= dcterms:description) |                     |            |
| Kommentar (= rdfs:comment)          |                     |            |
| Anvendelsesnote (= vann:usageNote)  |                     |            |
| Eksempel (= skos:example)           |                     |            |

Følgende metadata anvendes kun til beskrivelse af egenskaber:

<table>
<colgroup>
<col style="width: 55%" />
<col style="width: 22%" />
<col style="width: 22%" />
</colgroup>
<thead>
<tr class="header">
<th></th>
<th><strong>Vokabular</strong></th>
<th><strong>Profil</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Underegenskab af (= rdfs:subPropertyOf)</td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>Modsatrettet egenskab (= owl:inverseOf)</td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><blockquote>
<p>Ækvivalent egenskab (= owl:equivalentProperty)</p>
</blockquote></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>Domæne (= rdfs:domain)</td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>Udfaldsrum (= rdfs:range)</td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>Multiplicitet (= sh:minCount og/eller sh:maxCount)</td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

Følgende metadata anvendes kun til beskrivelse af klasser:

<table>
<colgroup>
<col style="width: 55%" />
<col style="width: 22%" />
<col style="width: 22%" />
</colgroup>
<thead>
<tr class="header">
<th></th>
<th><strong>Vokabular</strong></th>
<th><strong>Profil</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Underklasse af (= rdfs:subClassOf)</td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><blockquote>
<p>Ækvivalent klasse (= owl:equivalentClass)</p>
</blockquote></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

| **rdfs:isDefinedBy**                                                                                                                                                                                                                                                                                                       |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Det er god praksis at angive hvor et element har sin oprindelige definition fra. Dette angives oftest ved brug af metadata-egenskaben rdfs:isDefinedBy. Da 'isDefinedBy' reelt blot angiver navneområdet for elementet -- og derfor kan findes ved at følge dette -- så er den oplysning af undladt i anvendelsesprofilen. |

## Eksempler i dokumentet

Gennem dokumentet eksemplificeres profilens enkelte dele med eksempler.
Eksemplerne har taget åbent tilgængelige data fra en eksisterende
organisation og brugt dem til at vise en mulig udgave af en specifik del
af profilen. De anvendte data er hentet fra Tønder Kommunes hjemmeside
og er tolket efter bedste evne. Eksemplerne er ikke koordineret med
kommunen.

Ved hvert eksempel viser et diagram hvad der beskrives i koden og den
efterfølgende JSON-LD-kode viser hvordan eksemplet kunne se ud.

Som nævnt tidlige er basisprofilen defineret med RDF som fundament. RDF
kan udtrykkes i en bred vifte af konkrete formater, der så kan bruges
eksempelvis til udveksling af data mellem it-systemer. Til eksemplerne
er et RDF JSON-format anvendt, JSON-LD. JSO-LD er JSON og bør derfor
kunne genkendes af alle der tidligere har set eller anvendt JSON.

JSON-LD tilføjer en mapning til RDF ved hjælp af en såkaldt 'context'.
For at gøre de enkelte eksempler lettere at læse er denne context-del
undladt i de enkelte eksempler. Den samlede JSON-LD-graf med anvendte
eksempler og context er derfor gengivet i 'Bilag J -- JSON-LD
eksempelkode'.

Eksemplerne kan ses data hentet fra et fiktivt it-system der leverer
egne data i en form tilpasset basisprofil for organisation. Data der
skal fremstå som skabt i det fiktive system, er alle tildelt samme
navnerum: <https://data.gov.dk/model/profile/exampleorg/> der anvender
præfikset: 'xorg'.

# Repræsentation af identifikatorer og referencer

It-systemer forvaltet og anvendt af danske offentlige organisationer
anvender mange typer af koder. Enten til at identificerer et objekt i
systemet eller som reference til et objekt -- oftest eksternt i forhold
til it-systemet.

I relation til organisationsbeskrivende data anvendes cvr-nummer,
p-nummer og myndighedskode ofte som den identifikationskode -- eller
identifikator -- de er tænkt anvendt som. Men de anvendes også som andet
end en entydig identifikator for objektet. Eksempelvis kan et
adresse-objekt, have tilføjet en myndighedskode i form af en
kommunekode. Kommunekoden er i det tilfælde ikke en identifikator for
selve adresse-objektet, men bruges som en information om hvilken kommune
adressen ligger i. Myndighedskoden/kommunekoden bruges altså som en
reference til et andet objekt der har koden som identifikator.

Brugen af egenskaber, som cvr-nummer, p-nummer og myndighedskode, på den
beskrevne måde er ikke forkert -- **inden for det pågældende systems
rammer, med de regler og fortolkninger der er tilknyttet systemet.** Men
når de samme data bruges uden for systemet, så er der brug for en måde
at skelne mellem en egenskab der fungerer som identifikator for et
objekt og en egenskab der refererer til et (eksternt) objekt.

Når data skal indgå i en sammenhæng hvor semantisk interoperabilitet er
et mål, så bør så mange data som muligt gøres entydigt
maskinfortolkelige. Mere præcist udtrykt så bør det i basisprofilen
gøres klart hvornår en kode optræder som identifikator for et objekt og
hvornår koden er en reference til et objekt.

Basisprofilen anvender derfor

- både en type egenskab der repræsenterer cvr-nummer, p-nummer eller
  myndighedskode som værende identifikator for et objekt egenskaben
  bruges på

- samt en type egenskab der -- via cvr-nummer, p-nummer eller
  myndighedskode - fungerer som reference til et det objekt der
  identificeret med.

Dermed sikres der entydighed i tolkning samtidigt med at de to
eksisterende anvendelser -- og de bagvedliggende behov -- respekteres.

Til at repræsentere de tre typer af koder som identifikatorer vil
basisprofilen anvende en SEMIC-anvendt identifikatorklasse:
adms:Identifier. Dette beskrives nærmere i afsnittet *Standardisering af
tegnbaserede identifikatorer*.

Til a repræsentere koderne anvendt som referencer defineres følgende
egenskaber relateret til de tre identifikatorer cvr-nummer, p-nummer og
myndighedskode:

| **Beskrivelse**                         | **Forkortet URI**      | **URI (foreslået)**                                               |
| --------------------------------------- | ---------------------- | ----------------------------------------------------------------- |
| reference til objekt med cvr-nummer     | ovx:cvrCodeReference   | https://data.gov.dk/model/core/­org-extension/­cvrCodeReference   |
| reference til objekt med p-nummer       | ovx:pUnitCodeReference | https://data.gov.dk/model/core/­org-extension/­pUnitCodeReference |
| reference til objekt med myndighedskode | ovx:authCodeReference  | https://data.gov.dk/model/core/­org-extension/­authCodeReference  |

## Standardisering af tegnbaserede identifikatorer

Basisprofilen for organisation anvender den af EUs *Semantic
Interoperability Community* (SEMIC) [^1] definerede
adms:Identifier-klasse [^2]. Klassen er defineret med henblik på at have
en enkelt funktion, et enkelt element, til at repræsentere de mange
typer af tegnbaserede identifikatorer der anvendes på tværs af
organisationer, it-systemer og medlemslande. Klassen er defineret i
vokabularet *Asset Description Metadata Schema* (ADMS). Vokabularet
varetages af SEMIC-fællesskabet.

Klassen benyttes eksempelvis i SEMIC-vokabularer og anvendelsesprofiler,
herunder i *Core Person Vocabulary* [^3], *Core Public Organisation
Vocabulary* og *Core Business Vocabulary*. [^4]

I denne udgave af basisprofilen anvendes klassen til følgende
identifikatorer:

- cvr-nummer

- p-nummer

- myndighedskode (herunder 'kommunekode og 'regionskode')

- samt til lokal, organisatorisk bestemt identifikation af
  organisatorisk enhed

Brug af klassen adms:Identifier har til hensigt at give både
fleksibilitet og beriget information hvor identifikatorer anvendes.

### Anvendelse

Ressourcer eller objekter kan effektivt og entydigt identificeres ved
anvendelse af direkte 'resolverbare' HTTP-URIer. Disse URIer fungerer
ikke blot som entydige identifikatorer, men kan også bruges som link til
ressourcen eller objektet, hvorefter yderligere information om
ressourcen kan findes.

Etablerede it-systemer der ønskes inddraget i et miljø med semantisk
interoperabilitet kan ikke forventes at omdanne sine tegnbaserede
identifikatorer til resolverbare HTTP-URIer. Generelt kan brugen af
klassen adms:Identifier ses som en mulighed for at forbinde de
tegnbaserede identifikatorer med relevante maskinfortolkelige
informationer.

I SEMIC-regi gøres dette som vist her:

![](media/image3.emf){width="6.660869422572178in"
height="1.7201902887139107in"}

Egenskaben adms:identifier anvendes på det objekt (den ressource) der
har en tegnbaseret identifikator der skal beskrives. Klassen
adms:Identifier bruges i SEMIC-regi med fem egenskaber.:

<table>
<colgroup>
<col style="width: 34%" />
<col style="width: 65%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Egenskab</strong></th>
<th><strong>Beskrivelse</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>kode</p>
<blockquote>
<p>= skos:notation</p>
</blockquote></td>
<td><p>den tegnbaserede identifikator kombineret med en brugerdefineret
datatype.</p>
<p>Datatypen er en HTTP-URI der vil kunne bruges til at hente yderligere
beskrivelser om datatypen, eksempelvis RegEx mønstre.</p></td>
</tr>
<tr class="even">
<td><p>schema navn</p>
<blockquote>
<p>= rdfs:label</p>
</blockquote></td>
<td>navnet på det schema der fastlægger udformningen af
identifikatoren</td>
</tr>
<tr class="odd">
<td><p>schema URI</p>
<blockquote>
<p>= dcterms:conformsTo</p>
</blockquote></td>
<td>URI for det schema der fastlægger udformningen af
identifikatoren</td>
</tr>
<tr class="even">
<td><p>udstedende myndighed</p>
<blockquote>
<p>= adms:schemaAgency</p>
</blockquote></td>
<td>navn på den myndighed der har udstedt identifikatoren</td>
</tr>
<tr class="odd">
<td><p>udstedelsesdato</p>
<blockquote>
<p>= dcterms:issued</p>
</blockquote></td>
<td>dato for identifikatorens oprettelse</td>
</tr>
</tbody>
</table>

I 'Bilag G -- Brugerdefinerede datatyper' beskrives de tre datatyper der
er defineret til brug for henholdsvis cvr-nummer, p-nummer og
myndighedskode.

## Beskrivelse af klasse og egenskaber til identifikation

![](media/image4.emf){width="6.889232283464567in"
height="1.7043471128608925in"}

#### identifikator

##### Vokabularets definition og beskrivelser

| URI        | <http://www.w3.org/ns/adms#identifier>             |
| ---------- | -------------------------------------------------- |
| Term       | identifikator                                      |
| Kommentar  | Linker en ressource til en adms:Identifier-klasse. |
| Domæne     | rdfs:Resource                                      |
| Udfaldsrum | adms:Identifier                                    |

##### Profilens restriktioner og beskrivelser

| Foretrukken term | identifikator                                                              |
| ---------------- | -------------------------------------------------------------------------- |
| Definition       | Linker en ressource til en adms:Identifier-klasse                          |
| Domæne           | org:FormalOrganization eller org:OrganizationalUnit eller dcterms:Location |
| Udfaldsrum       | adms:Identifier                                                            |
| Multiplicitet    | 0 - \*                                                                     |

### Identifikator (klasse)

![](media/image5.emf){width="4.008695319335083in"
height="1.6867410323709537in"}

##### Vokabularets definition og beskrivelser

| URI       | <http://www.w3.org/ns/adms#Identifier>            |
| --------- | ------------------------------------------------- |
| Term      | Identifkator                                      |
| Kommentar | Dette er baseret på UN/CEFACT Identifier-klassen. |

##### Profilens restriktioner og beskrivelser

<table>
<colgroup>
<col style="width: 22%" />
<col style="width: 77%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th>identifkator</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Definition</td>
<td>En struktureret reference, der identificerer en entitet.</td>
</tr>
<tr class="even">
<td>Anvendelsesnote</td>
<td><p>[fra ADMS Vocabulary-websiden]</p>
<p>En identifikator i en bestemt kontekst, bestående af</p>
<ul>
<li><p>indholdsstreng, der er identifikatoren;</p></li>
<li><p>en valgfri identifikator for identifikationssystemet;</p></li>
<li><p>en valgfri identifikator for versionen af
identifikationsskemaet;</p></li>
<li><p>en valgfri identifikator forden organisation, der administrerer
identifikationsordningen.</p></li>
</ul></td>
</tr>
<tr class="odd">
<td>Anvendelsesnote</td>
<td>Klassen adms:Identifier anvendes i denne udgave af basisprofilen til
følgende identifikatorer: cvr-nummer, p-nummer og myndighedskode, samt
til lokalt/organisatorisk definerede brugervendte nøgler for
organisatoriske enheder.</td>
</tr>
</tbody>
</table>

#### notation

##### Vokabularets definition og beskrivelser

| URI             | <http://www.w3.org/2004/02/skos/core#notation>                                                                                                                                                            |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Term            | notation                                                                                                                                                                                                  |
| Definition      | En notation, også kendt som klassifikationskode, er en streng af tegn såsom \"T58.5\" eller \"303.4833\", der bruges til entydigt at identificere et begreb inden for rammerne af et givet begrebssystem. |
| Anvendelsesnote | Efter konvention bruges skos:notation med en typeangivet literal i objekt-positionen af en triple.                                                                                                        |
| Domæne          | rdfs:Resource                                                                                                                                                                                             |
| Udfaldsrum      | rdfs:Resource                                                                                                                                                                                             |

##### Profilens restriktioner og beskrivelser

| Foretrukken term | kode                                                                                                            |
| ---------------- | --------------------------------------------------------------------------------------------------------------- |
| Anvendelsesnote  | En streng, der er en identifikator i sammenhæng med identifikationsskemaet, der refereres til af dens datatype. |
| Domæne           | rdfs:Resource                                                                                                   |
| Udfaldsrum       | rdfs:Literal                                                                                                    |
| Multiplicitet    | 1 - 1                                                                                                           |

#### schema navn

##### Vokabularets definition og beskrivelser

| URI        | <http://www.w3.org/2000/01/rdf-schema#label> |
| ---------- | -------------------------------------------- |
| Term       | betegnelse                                   |
| Kommentar  | Et menneskelæsbart navn for emnet.           |
| Domæne     | rdfs:Resource                                |
| Udfaldsrum | rdfs:Literal                                 |

##### Profilens restriktioner og beskrivelser

| Foretrukken term | betegnelse                                                           |
| ---------------- | -------------------------------------------------------------------- |
| Alternativ term  | schema navn                                                          |
| Anvendelsesnote  | Navn på det skema, der blev brugt til at konstruere identifikatoren. |
| Domæne           | adms:Identifier                                                      |
| Udfaldsrum       | rdf:langString                                                       |
| Multiplicitet    | 0 - \*                                                               |

#### udstedelsesdato

##### Vokabularets definition og beskrivelser

| URI              | <http://purl.org/dc/terms/issued>                                   |
| ---------------- | ------------------------------------------------------------------- |
| Term             | udstedelsesdato                                                     |
| Kommentar        | Dato for formel udstedelse (f.eks. offentliggørelse) af ressourcen. |
| Domæne           | rdfs:Resource                                                       |
| Udfaldsrum       | rdfs:Literal                                                        |
| Underegenskab af | dcterms:date                                                        |

##### Profilens restriktioner og beskrivelser

| Foretrukken term | udstedelsesdato                              |
| ---------------- | -------------------------------------------- |
| Anvendelsesnote  | Den dato, hvor identifikatoren blev tildelt. |
| Domæne           | adms:Identifier                              |
| Udfaldsrum       | xsd:date                                     |
| Multiplicitet    | 0 - 1                                        |

#### udstedende myndighed

##### Vokabularets definition og beskrivelser

| URI        | <http://www.w3.org/ns/adms#schemaAgency>                     |
| ---------- | ------------------------------------------------------------ |
| Term       | skemaorganisation                                            |
| Kommentar  | Navnet på det organisation, der har udstedt identifikatoren. |
| Domæne     | adms:Identifier                                              |
| Udfaldsrum | rdfs:Literal                                                 |

##### Profilens restriktioner og beskrivelser

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th>udstedende myndighed</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Definition</td>
<td><p>[fra Core Public Organisation Vocabulary websiden]</p>
<p>Navnet på den autoritet, der er ansvarlig for at udstede
identifikatoren.</p></td>
</tr>
<tr class="even">
<td>Domæne</td>
<td>adms:Identifier</td>
</tr>
<tr class="odd">
<td>Udfaldsrum</td>
<td>rdf:langString</td>
</tr>
<tr class="even">
<td>Multiplicitet</td>
<td>0 - *</td>
</tr>
</tbody>
</table>

#### schema URI

##### Vokabularets definition og beskrivelser

| URI              | <http://purl.org/dc/terms/conformsTo>                                         |
| ---------------- | ----------------------------------------------------------------------------- |
| Term             | er i overensstemmelse med                                                     |
| Kommentar        | En etableret standard, som den beskrevne ressource er i overensstemmelse med. |
| Underegenskab af | dcterms:relation                                                              |
| Domæne           | rdfs:Resource                                                                 |
| Udfaldsrum       | dcterms:Standard                                                              |

##### Profilens restriktioner og beskrivelser

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th>schema URI</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Beskrivelse</td>
<td><p>[fra Core Public Organisation Vocabulary websiden]</p>
<p>URI for det skema, der bruges til at konstruere
identifikatoren.</p></td>
</tr>
<tr class="even">
<td>Anvendelsesnote</td>
<td>URIen angives i form af en tekststreng.</td>
</tr>
<tr class="odd">
<td>Domæne</td>
<td>adms:Identifier</td>
</tr>
<tr class="even">
<td>Udfaldsrum</td>
<td>xsd:anyURI</td>
</tr>
<tr class="odd">
<td>Multiplicitet</td>
<td>0 - *</td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="media/image6.png"
style="width:0.19335in;height:0.178in" />
<strong>Important</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Bemærk at SEMIC angiver at egenskaben dcterms:conformsTo kan have
xsd:anyURI som udfaldsrum. Det synes at stride imod Dublin Core Terms
definitionen hvor ’range’ er dcterms:Standard (en klasse). Egenskaben
dcterms:conformsTo er en underegenskab til dcterms:relation og må derfor
ikke være i konflikt med denne. I en note til egenskaben
dcterms:relation hedder det: ”Dette udtryk er beregnet til at blive
brugt med non-Literal værdier som defineret i DCMI Abstract Model (<a
href="http://dublincore.org/documents/abstract-model/).%E2%80%9D">http://dublincore.org/documents/abstract-model/).”</a>
Datatypen xsd:anyURI er en Literal.</p>
<p>I denne udgave af basisprofilen er det valgt indtil videre at
fastholde brugen af xsd:anyURI mens en afklaring i SEMIC-regi forsøges
opnået.</p></td>
</tr>
</tbody>
</table>

## Eksempler på identifikatorer

Herunder vises hvordan tre af Tønder Kommunes identifikatorer kan
udtrykkes ved brug af adms:Identifier. Til illustration vil kommunens
cvr-nummer, et p-nummer og myndighedskoden blive anvendt.

##### Tønder Kommunes cvr-nummer 29189781:

| **Egenskab**         | **værdi**                 |
| -------------------- | ------------------------- |
| kode                 | 29189781\^\^id-dk:cvrCode |
| schema navn          | Cvr-nummer                |
| schema URI \*)       |                           |
| udstedende myndighed | Danmarks Statistik        |
| udstedelsesdato      |                           |

\*) Der er ikke fundet noget officielt schema der definerer
'cvr-nummer'.

##### Tønder Kommunes p-nummer 1003326862:

| **Egenskab**         | **værdi**                     |
| -------------------- | ----------------------------- |
| kode                 | 1003326862\^\^id-dk:pUnitCode |
| schema navn          | P-nummer                      |
| schema URI \*)       |                               |
| udstedende myndighed | Danmarks Statistik            |
| udstedelsesdato      |                               |

\*) Der er ikke fundet noget officielt schema der definerer 'P-nummer'.

##### Tønder Kommunes p-nummer myndighedskode:

| **Egenskab**         | **Værdi**                          |
| -------------------- | ---------------------------------- |
| kode                 | 0550\^\^id-dk:authCode             |
| schema navn          | Myndighedskode                     |
| schema URI \*)       |                                    |
| udstedende myndighed | CPR -- Det centrale Personregister |
| udstedelsesdato      |                                    |

\*) Der er ikke fundet noget officielt schema der definerer
'Myndighedskode'.

![](media/image7.emf)

##### JSON-LD-kode (uden context)

{

\"@id\" : \"xorg:org-844\",

\"@type\" : \"org:FormalOrganization\",

\"identifier\" : \[ \"xorg:id-888\", \"xorg:Id-956\", \"xorg:id-714\"
\],

}

{

\"@id\" : \"xorg:Id-956\",

\"@type\" : \"adms:Identifier\",

\"issued\" : \"2007-01-01\",

\"label\" : \"Cvr-nummer\",

\"notation\" : \"29189781\^\^id-dk:cvrCode\",

\"schemaAgency\" : {

\"@language\" : \"da\",

\"@value\" : \"Danmarks Statistik\"

}

}

{

\"@id\" : \"xorg:id-714\",

\"@type\" : \"adms:Identifier\",

\"issued\" : \"1993-01-01\",

\"label\" : \"P-nummer\",

\"notation\" : \"1003326862\^\^id-dk:pUnitCode\",

\"schemaAgency\" : {

\"@language\" : \"da\",

\"@value\" : \"Danmarks Statistik\"

}

}

{

\"@id\" : \"xorg:id-888\",

\"@type\" : \"adms:Identifier\",

\"label\" : \"Myndighedskode\",

\"notation\" : \"0550\^\^id-dk:authCode\",

\"schemaAgency\" : {

\"@language\" : \"da\",

\"@value\" : \"CPR -- Det centrale Personregister\"

}

}

# Organisationen og den organisatoriske struktur

Basisprofilens to centrale elementer er klassen for organisationer og
klassen for organisatoriske enheder. Til at repræsentere disse benyttes
to klasser fra vokabularet Organization Ontology: org:FormalOrganization
(=Organisation) og org:OrganizationalUnit (= Organisatorisk enhed).

![](media/image8.emf){width="5.165217629046369in"
height="0.7562084426946631in"}

Organisationen beskrives i afsnittet 'Organisationen og dens
egenskaber'.

Den organisatoriske enhed beskrives i afsnittet 'Den organisatoriske
enhed og dens egenskaber'.

Organisationer vil i de fleste tilfælde have en organisatorisk struktur,
oftest i en hierarkisk form, hvor organisationen er opdelt i mindre
organisatoriske enheder. Organisationer består typisk af afdelinger,
kontorer, enheder, teams, grupper osv. En organisationsenhed kan i sig
selv have underordnede enheder. Den interne struktur i form af forholdet
mellem organisation og organisatoriske enheder beskrives i afsnittet
'Organisationen og dens dele'.

Organisationer kan også have relationer til andre organisationer.
Eksempelvis kan et ministerium bestå af flere underordnede styrelser.
Både ministeriet og dets styrelser er hver for sig selvstændige
organisationer. Organisationer kan indbyrdes have andre former for
relationer end de der udtrykkes i form af under- og overorganisatoriske
forhold, fx finansiering eller kæderelationer. Organisationers indbyrdes
relation beskrives i afsnittet 'Organisationens relationer til andre
organisationer'.

## Organisationens tilhørende enheder

![](media/image9.emf){width="4.045742563429571in"
height="2.686956474190726in"}

#### har enhed

##### *Vokabularets definition og beskrivelser*

| URI                   | http://www.w3.org/ns/org#hasUnit                                                                |
| --------------------- | ----------------------------------------------------------------------------------------------- |
| Term                  | har enhed                                                                                       |
| Kommentar             | Angiver en enhed, som er del af denne organisation, f.eks. en afdeling i en større organisation |
| Domæne                | org:FormalOrganization                                                                          |
| Udfaldsrum            | org:OrganizationalUnit                                                                          |
| Underegenskab af      | org:hasSubOrganization                                                                          |
| Modsatrettet egenskab | org:unitOf                                                                                      |

##### Profilens restriktioner og beskrivelser {#profilens-restriktioner-og-beskrivelser-7}

| Foretrukken term | har enhed                                                                                       |
| ---------------- | ----------------------------------------------------------------------------------------------- |
| Definition       | Angiver en enhed, som er del af denne organisation, f.eks. en afdeling i en større organisation |
| Domæne           | org:FormalOrganization                                                                          |
| Udfaldsrum       | org:OrganizationalUnit                                                                          |
| Multiplicitet    | 0 - \*                                                                                          |

#### enhed af

##### *Vokabularets definition og beskrivelser*

| URI                   | <http://www.w3.org/ns/org#unitOf>                                                                                 |
| --------------------- | ----------------------------------------------------------------------------------------------------------------- |
| Term                  | enhed af                                                                                                          |
| Kommentar             | Angiver en organisation, som denne enhed er en del af, f.eks. en afdeling inden for en større formel organisation |
| Domæne                | org:OrganizationalUnit                                                                                            |
| Udfaldsrum            | org:Organization                                                                                                  |
| Underegenskab af      | org:subOrganizationOf                                                                                             |
| Modsatrettet egenskab | org:hasUnit                                                                                                       |

##### Profilens restriktioner og beskrivelser {#profilens-restriktioner-og-beskrivelser-8}

| Foretrukken term | enhed af                                                                                                                                 |
| ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| Definition       | Angiver en organisation, som denne enhed er en del af, f.eks. en afdeling inden for en større formel organisation                        |
| Kommentar        | Angiver en formel organisation, som denne organisatoriske enhed er en del af, f.eks. en afdeling inden for en større formel organisation |
| Anvendelsesnote  | En organisatorisk enhed skal altid være tilknyttet en og kun en formel organisation.                                                     |
| Domæne           | org:OrganizationalUnit                                                                                                                   |
| Udfaldsrum       | org:FormalOrganization                                                                                                                   |
| Multiplicitet    | 1 - 1                                                                                                                                    |

#### har øvre enhed

##### *Vokabularets definition og beskrivelser*

| URI                   | https://data.gov.dk/model/core/orgextension/hasUpperUnit                        |
| --------------------- | ------------------------------------------------------------------------------- |
| Term                  | har øvre enhed                                                                  |
| Definition            | Angive en enhed der er øverst i den formelle organisations hierarkiske struktur |
| Domæne                | org:FormalOrganization                                                          |
| Udfaldsrum            | org:OrganizationalUnit                                                          |
| Underegenskab af      | org:hasUnit                                                                     |
| Modsatrettet egenskab | ovx:upperUnitOf                                                                 |

##### *Profilens restriktioner og beskrivelser* {#profilens-restriktioner-og-beskrivelser-9}

| Foretrukken term | øvre enhed i           |
| ---------------- | ---------------------- |
| Alternativ term  | topenhed i             |
| Domæne           | org:OrganizationalUnit |
| Udfaldsrum       | org:FormalOrganization |
| Multiplicitet    | 0 -- 1                 |

#### øvre enhed i

##### *Vokabularets definition og beskrivelser*

| URI                   | https://data.gov.dk/model/core/orgextension/upperUnitOf                                                        |
| --------------------- | -------------------------------------------------------------------------------------------------------------- |
| Term                  | øvre enhed i                                                                                                   |
| Definition            | Angivelse af den formelle organisation hvori enheden er placeret på øverste niveau i den hierarkiske struktur. |
| Domæne                | org:OrganizationalUnit                                                                                         |
| Udfaldsrum            | org:FormalOrganization                                                                                         |
| Underegenskab af      | org:unitOf                                                                                                     |
| Modsatrettet egenskab | ovx:hasUpperUnit                                                                                               |

##### *Profilens restriktioner og beskrivelser* {#profilens-restriktioner-og-beskrivelser-10}

| Foretrukken term | øvre enhed i           |
| ---------------- | ---------------------- |
| Alternativ term  | topenhed i             |
| Domæne           | org:OrganizationalUnit |
| Udfaldsrum       | org:FormalOrganization |
| Multiplicitet    | 0 -- 1                 |

## Organisatoriske enheders indbyrdes hierarki

![](media/image10.emf){width="1.9771161417322836in"
height="1.1739129483814523in"}

#### enhed af

##### *Vokabularets definition og beskrivelser*

| URI                   | <http://www.w3.org/ns/org#unitOf>                                                                                 |
| --------------------- | ----------------------------------------------------------------------------------------------------------------- |
| Term                  | enhed af                                                                                                          |
| Kommentar             | Angiver en organisation, som denne enhed er en del af, f.eks. en afdeling inden for en større formel organisation |
| Anvendelsesnote       | Dette er den inverse egenskab af org:hasUnit.                                                                     |
| Domæne                | org:OrganizationalUnit                                                                                            |
| Udfaldsrum            | org:Organization                                                                                                  |
| Underegenskab af      | org:subOrganizationOf                                                                                             |
| Modsatrettet egenskab | org:hasUnit                                                                                                       |

##### Profilens restriktioner og beskrivelser {#profilens-restriktioner-og-beskrivelser-11}

<table>
<colgroup>
<col style="width: 22%" />
<col style="width: 77%" />
<col style="width: 0%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th>enhed af</th>
<th></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Definition</td>
<td>Angiver en organisationatorisk enhed, som denne enhed er en del
af</td>
<td></td>
</tr>
<tr class="even">
<td>Kommentar</td>
<td colspan="2"><p>en organisationsenhed kan være underlagt en anden
organisationsenhed</p>
<p>en organisationsenhed kan indeholde 0 en eller flere
enheder.</p></td>
</tr>
<tr class="odd">
<td>Eksempel</td>
<td colspan="2"><p>en afdeling i en større division</p>
<p>et team i en afdeling</p></td>
</tr>
<tr class="even">
<td>Anvendelsesnote</td>
<td colspan="2">Anvendes fra ’Organisatorisk enhed’ til at angive en
enhed (i samme organisation) som den anvende enhed er organisatorisk
underlagt.</td>
</tr>
<tr class="odd">
<td>Domæne</td>
<td colspan="2">org:OrganizationalUnit</td>
</tr>
<tr class="even">
<td>Udfaldsrum</td>
<td colspan="2">org:OrganizationalUnit</td>
</tr>
<tr class="odd">
<td>Multiplicitet</td>
<td colspan="2">1 - 1</td>
</tr>
</tbody>
</table>

## Eksempel på organisation og enheders relationer

![](media/image11.emf)

##### JSON-LD-kode (uden context)

{

{

\"@id\" : \"xorg:unit-864\",

\"@type\" : \"org:OrganizationalUnit\",

\"label\" : \"unit-864\",

\"prefLabel\" : {

\"@language\" : \"da\",

\"@value\" : \"Borgerservice\"

},

\"unitOf\" : \"xorg:org-844\",

}

{

\"@id\" : \"xorg:unit-570\",

\"@type\" : \"org:OrganizationalUnit\",

\"label\" : \"unit-570\",

\"prefLabel\" : {

\"@language\" : \"da\",

\"@value\" : \"Skærbæk Borgerservice\"

},

\"unitOf\" : \[ \"xorg:org-844\", \"xorg:unit-864\" \],

}

{

\"@id\" : \"xorg:unit-931\",

\"@type\" : \"org:OrganizationalUnit\",

\"label\" : \"unit-931\",

\"prefLabel\" : {

\"@language\" : \"da\",

\"@value\" : \"Direktion\"

},

\"upperUnitOf\" : \"xorg:org-844\",

}

}

# Organisationens relationer til andre organisationer

Relationer organisationer imellem beskrives i basisprofilen som
kvalificeret relation via klassen ovx:Relation . I vokabularet
Organizational Ontology kan disse typer af forbindelser beskrives enten
ved brug af org:subOrganizationOf eller org:linkedTo. De beskriver
henholdsvis at en organisation er 'underorganisation' til en anden
organisation eller at en organisation har en relation af udefineret art
til en anden organisation.

For at kunne opfylde behovet for beskrivelse af et bredere felt af
relationer organisationer i mellem, gør profilen brug af følgende
struktur til at give mere uddybende information end de de kan gives med
org:subOrganizationOf og org:linkedTo.

![](media/image12.emf){width="6.06869094488189in" height="3.2in"}

### Relation (klasse)

##### *Vokabularets definition og beskrivelser*

| URI              | https://data.gov.dk/model/core/orgextension/Relation              |
| ---------------- | ----------------------------------------------------------------- |
| Term             | Relation                                                          |
| Foretrukken term | Relation                                                          |
| Definition       | Angiver to organisationer samt typen af deres indbyrdes relation. |

##### 

#### startede

##### *Vokabularets definition og beskrivelser*

| URI        | http://www.w3.org/ns/prov#startedAtTime                                                                                                                                                                                                                                                                                                                                            |
| ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Term       | startede                                                                                                                                                                                                                                                                                                                                                                           |
| Kommentar  | Start er, når en aktivitet anses for at være startet af en enhed, kendt som trigger. Aktiviteten eksisterede ikke før dens start. Enhver brug, generering eller ugyldiggørelse, der involverer en aktivitet, følger aktivitetens start. En start kan referere til en triggerentitet, der udløste aktiviteten, eller til en aktivitet, kendt som starter, der genererede triggeren. |
| Domæne     | [prov:Activity](https://www.w3.org/TR/2013/REC-prov-o-20130430/#Activity)                                                                                                                                                                                                                                                                                                          |
| Udfaldsrum | xsd:dateTime                                                                                                                                                                                                                                                                                                                                                                       |

##### *Profilens restriktioner og beskrivelser* {#profilens-restriktioner-og-beskrivelser-12}

| Foretrukken term | startede                                                                                                                                                                                                                                                                                                                                                                           |
| ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Definition       | Start er, når en aktivitet anses for at være startet af en enhed, kendt som trigger. Aktiviteten eksisterede ikke før dens start. Enhver brug, generering eller ugyldiggørelse, der involverer en aktivitet, følger aktivitetens start. En start kan referere til en triggerentitet, der udløste aktiviteten, eller til en aktivitet, kendt som starter, der genererede triggeren. |
| Anvendelsesnote  | Angiver den dato en relation mellem to organisationer blev etableret.                                                                                                                                                                                                                                                                                                              |
| Domæne           | ovx:Relation                                                                                                                                                                                                                                                                                                                                                                       |
| Udfaldsrum       | xsd:dateTime                                                                                                                                                                                                                                                                                                                                                                       |
| Multiplicitet    | 0 - 1                                                                                                                                                                                                                                                                                                                                                                              |

#### sluttede

##### *Vokabularets definition og beskrivelser*

| URI        | <http://www.w3.org/ns/prov#endedAtTime>                                                                                                                                                                                                                                                                                                                                                                           |
| ---------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Term       | sluttede                                                                                                                                                                                                                                                                                                                                                                                                          |
| Kommentar  | Slut er, når en aktivitet anses for at være afsluttet af en enhed, kendt som trigger. Aktiviteten eksisterer ikke længere efter dens afslutning. Enhver brug, generering eller ugyldiggørelse, der involverer en aktivitet, går forud for aktivitetens afslutning. En afslutning kan referere til en triggerenhed, der afsluttede aktiviteten, eller til en aktivitet, kendt som ender, der genererede triggeren. |
| Domæne     | prov:Activity                                                                                                                                                                                                                                                                                                                                                                                                     |
| Udfaldsrum | xsd:dateTime                                                                                                                                                                                                                                                                                                                                                                                                      |

##### *Profilens restriktioner og beskrivelser* {#profilens-restriktioner-og-beskrivelser-13}

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th><blockquote>
<p>sluttede</p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Definition</td>
<td>Slut er, når en aktivitet anses for at være afsluttet af en enhed,
kendt som trigger. Aktiviteten eksisterer ikke længere efter dens
afslutning. Enhver brug, generering eller ugyldiggørelse, der involverer
en aktivitet, går forud for aktivitetens afslutning. En afslutning kan
referere til en triggerenhed, der afsluttede aktiviteten, eller til en
aktivitet, kendt som ender, der genererede triggeren.</td>
</tr>
<tr class="even">
<td>Anvendelsesnote</td>
<td>Angiver den dato en relation mellem to organisationer blev
afsluttet.</td>
</tr>
<tr class="odd">
<td>Domæne</td>
<td>ovx:Relation</td>
</tr>
<tr class="even">
<td>Udfaldsrum</td>
<td>xsd:dateTime</td>
</tr>
<tr class="odd">
<td>Multiplicitet</td>
<td>0 - 1</td>
</tr>
</tbody>
</table>

#### har relation

| URI                   | https://data.gov.dk/model/core/orgextension/hasRelation           |
| --------------------- | ----------------------------------------------------------------- |
| Term                  | has relation                                                      |
| Foretrukken term (da) | har relation                                                      |
| Definition            | angiver en relation en organisation har til en anden organisation |
| Domæne                | org:FormalOrganization                                            |
| Udfaldsrum            | ovx:Relation                                                      |

#### relation til

| URI                   | https://data.gov.dk/model/core/orgextension/relationTo                            |
| --------------------- | --------------------------------------------------------------------------------- |
| Term                  | relationTo                                                                        |
| Foretrukken term (da) | relation til                                                                      |
| Definition            | angiver en organisation der er 'modtager' i en relation til en anden organisation |
| Domæne                | ovx:Relation                                                                      |
| Udfaldsrum            | org:FormalOrganization                                                            |

#### type

##### *Vokabularets definition og beskrivelser*

| URI         | http://purl.org/dc/terms/type                                                                                                                                                                                    |
| ----------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Term        | type                                                                                                                                                                                                             |
| Kommentar   | Ressourcens art eller genre.                                                                                                                                                                                     |
| Beskrivelse | Anbefalet bedste praksis er at bruge et kontrolleret ordforråd, såsom DCMI Type Vocabulary \[DCMITYPE\]. For at beskrive ressourcens filformat, fysiske medium eller dimensioner skal du bruge Format-elementet. |
| Domæne      | rdfs:Resource                                                                                                                                                                                                    |
| Udfaldsrum  | rdfs:Class                                                                                                                                                                                                       |

##### Profilens restriktioner og beskrivelser {#profilens-restriktioner-og-beskrivelser-14}

| Foretrukken term | type                                        |
| ---------------- | ------------------------------------------- |
| Definition       | Ressourcens art eller genre.                |
| Anvendelsesnote  | Angiver den type af relation der er tale om |
| Domæne           | ovx:Relation                                |
| Udfaldsrum       | ort:OrganizationalRelationType              |
| Multiplicitet    | 1                                           |

### Type af organisatorisk relation (klasse)

![](media/image13.emf){width="3.3275929571303586in"
height="1.408695319335083in"}

##### *Vokabularets definition og beskrivelser*

| URI              | https://data.gov.dk/concept/core/orgrelation/OrganizationalRelationType |
| ---------------- | ----------------------------------------------------------------------- |
| Term             | Type af organisatorisk relation                                         |
| Foretrukken term | Type af organisatorisk relation                                         |
| Definition       | Klassen af organisatoriske relationstyper                               |
| Underklasse af   | skos:Concept                                                            |

#### foretrukken term

##### *Vokabularets definition og beskrivelser*

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>URI</th>
<th><a
href="http://www.w3.org/2004/02/skos/core#prefLabel">http://www.w3.org/2004/02/skos/core#prefLabel</a></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Term</td>
<td>foretrukken term</td>
</tr>
<tr class="even">
<td>Definition</td>
<td>Den foretrukne leksikalske betegnelse for en ressource på et givet
sprog.</td>
</tr>
<tr class="odd">
<td>Kommentar</td>
<td><p>En ressource har ikke mere end én værdi af skos:prefLabel pr.
sprogtag.</p>
<p>Range for skos:prefLabel er klassen af RDF ’plain literals’.</p>
<p>skos:prefLabel, skos:altLabel og skos:hiddenLabel er parvis disjunkte
egenskaber.</p></td>
</tr>
<tr class="even">
<td>Domæne</td>
<td>rdfs:Resource</td>
</tr>
<tr class="odd">
<td>Udfaldsrum</td>
<td>xsd:string eller rdf:langString (tidligere angivet som
rdf:PlainLiteral)</td>
</tr>
<tr class="even">
<td>Underegenskab af</td>
<td>rdfs:label</td>
</tr>
</tbody>
</table>

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-15}

| Foretrukken term | foretrukken term               |
| ---------------- | ------------------------------ |
| Domæne           | ort:OrganizationalRelationType |
| Udfaldsrum       | rdf:langString                 |
| Multiplicitet    | 1 - \*                         |

#### definition

##### *Vokabularets definition og beskrivelser*

| URI              | http://www.w3.org/2004/02/skos/core#definition                    |
| ---------------- | ----------------------------------------------------------------- |
| Term             | definition                                                        |
| Definition       | En erklæring eller formel forklaring af betydningen af et begreb. |
| Underegenskab af | skos:note                                                         |
| Domæne           | rdfs:Resource                                                     |
| Udfaldsrum       | rdfs:Resource                                                     |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-16}

| Foretrukken term | definition                     |
| ---------------- | ------------------------------ |
| Anvendelsesnote  | Beskrivelse af relationstypen. |
| Domæne           | ort:OrganizationalRelationType |
| Udfaldsrum       | rdf:langString                 |
| Multiplicitet    | 0 - \*                         |

#### eksempel

##### *Vokabularets definition og beskrivelser*

| URI              | http://www.w3.org/2004/02/skos/core#example |
| ---------------- | ------------------------------------------- |
| Term             | eksempel                                    |
| Definition       | Et eksempel på brugen af et begreb.         |
| Underegenskab af | skos:note                                   |
| Domæne           | rdfs:Resource                               |
| Udfaldsrum       | rdfs:Resource                               |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-17}

| Foretrukken term | eksempel                            |
| ---------------- | ----------------------------------- |
| Definition       | En der illustrere typen af relation |
| Domæne           | ort:OrganizationalRelationType      |
| Udfaldsrum       | rdf:langString                      |
| Multiplicitet    | 0 - \*                              |

## Eksempel på en organisations relation til en anden

![](media/image14.emf)

##### JSON-LD-kode (uden context)

{

{

\"@id\" : \"xorg:org-844\",

\"@type\" : \"org:FormalOrganization\",

\"hasRelation\" : \"xorg:rel-314\",

}

{

\"@id\" : \"xorg:rel-314\",

\"@type\" : \"ovx:Relation\",

\"type\" : \"orl:memberOfInterestOrganization\",

\"prefLabel\" : {

\"@language\" : \"da\",

\"@value\" : \"Medlemskab af KL\"

},

\"startedAtTime\" : \"2007-01-01T00:00:00.00\",

\"relationTo\" : \"xorg:org-552\"

}

{

\"@id\" : \"xorg:org-552\",

\"@type\" : \"org:FormalOrganization\",

\"altLabel\" : \"KL\",

\"prefLabel\" : \[ {

\"@language\" : \"da\",

\"@value\" : \"Kommunernes Landsforening\"

}, {

\"@language\" : \"en\",

\"@value\" : \"Local Government Denmark\"

} \]

}

}

# Organisation og dens egenskaber

![](media/image15.emf){width="6.693692038495188in"
height="2.7565212160979877in"}

## Klassen Organisation

![](media/image16.emf){width="2.365217629046369in"
height="0.8256583552055993in"}

##### *Vokabularets definition og beskrivelser*

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>URI</th>
<th><a
href="http://www.w3.org/ns/org#FormalOrganization">http://www.w3.org/ns/org#FormalOrganization</a></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Term</td>
<td>Formel organisation</td>
</tr>
<tr class="even">
<td>Kommentar</td>
<td>En organisation, der er anerkendt i verden bredt set, især i
juridiske jurisdiktioner, med tilhørende rettigheder og ansvar.
Eksempler inkluderer et selskab, velgørenhed, regering eller kirke.</td>
</tr>
<tr class="odd">
<td>Anvendelsesnote</td>
<td>Bemærk, at dette er en superklasse af `gr:BusinessEntity`, og det
anbefales at bruge GoodRelations-vokabularet til at betegne
Business-klassifikationer såsom DUNS eller NAICS.</td>
</tr>
<tr class="even">
<td>Underklasse af</td>
<td><p>foaf:Organization</p>
<p>org:Organization</p></td>
</tr>
</tbody>
</table>

##### Profilens restriktioner og beskrivelser {#profilens-restriktioner-og-beskrivelser-18}

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th>Formel organisation</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Alternativ term</td>
<td>Organisation</td>
</tr>
<tr class="even">
<td>Definition</td>
<td>En organisation, der er anerkendt i verden bredt set, især i
juridiske jurisdiktioner, med tilhørende rettigheder og ansvar.</td>
</tr>
<tr class="odd">
<td>Eksempel</td>
<td><p>et aktieselskab</p>
<p>en statslig styrelse</p>
<p>en velgørende forening</p>
<p>en kirkelig forening</p>
<p>....</p></td>
</tr>
<tr class="even">
<td>Kommentar</td>
<td><p>Organisationer kan ofte nedbrydes i hierarkiske strukturer</p>
<p>Organisationen er "rammen" for alle de øvrige elementer
(Organisationsenheder, Organisationsmedlemmer og deres indbyrdes
relationer)</p></td>
</tr>
</tbody>
</table>

## Egenskaber for Organisation

![](media/image17.emf){width="4.382608267716535in"
height="1.8602569991251094in"}

#### foretrukken term

##### *Vokabularets definition og beskrivelser*

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>URI</th>
<th><a
href="http://www.w3.org/2004/02/skos/core#prefLabel">http://www.w3.org/2004/02/skos/core#prefLabel</a></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Term</td>
<td>foretrukken term</td>
</tr>
<tr class="even">
<td>Definition</td>
<td>Den foretrukne leksikalske betegnelse for en ressource på et givet
sprog.</td>
</tr>
<tr class="odd">
<td>Kommentar</td>
<td><p>En ressource har ikke mere end én værdi af skos:prefLabel pr.
sprogtag.</p>
<p>Range for skos:prefLabel er klassen af RDF ’plain literals’.</p>
<p>skos:prefLabel, skos:altLabel og skos:hiddenLabel er parvis disjunkte
egenskaber.</p></td>
</tr>
<tr class="even">
<td>Domæne</td>
<td>rdfs:Resource</td>
</tr>
<tr class="odd">
<td>Udfaldsrum</td>
<td>xsd:string eller rdf:langString (tidligere angivet som
rdf:PlainLiteral)</td>
</tr>
<tr class="even">
<td>Underegenskab af</td>
<td>rdfs:label</td>
</tr>
</tbody>
</table>

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-19}

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th>foretrukken term</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Kommentar</td>
<td>Alment anvendt navn for en organisation .Ofte vil organisationens
navn være det samme som man finder i CVR-registret eller
Myndighedsregistret, når der er tale om virksomheders og myndigheders
navne.</td>
</tr>
<tr class="even">
<td>Anvendelsesnote</td>
<td>Den foretrukne leksikalske betegnelse for en formel organisation,
Bruges til at angive organisationens primære - ofte juridisk anerkendte
- navn. Det antages at organisationer kun har et enkelt navn eller en
enkelt betegnelse som det foretrukne, eventuelt med oversatte versioner
på andre sprog. Med andre ord kan primære navne angives på flere sprog
og dermed give flere forekomster af egenskaben skos:prefLabel for den
enkelte organisation.</td>
</tr>
<tr class="odd">
<td>Eksempel</td>
<td><p>"Digitaliseringsstyrelsen"</p>
<p>"Næstved Sygehus"</p>
<p>"Holbæk kommune"</p>
<p>"FDF-spejderne i Vejle"</p></td>
</tr>
<tr class="even">
<td>Udfaldsrum</td>
<td>rdf:langString</td>
</tr>
<tr class="odd">
<td>Multiplicitet</td>
<td>1 - *</td>
</tr>
</tbody>
</table>

#### alternativ term

##### *Vokabularets definition og beskrivelser*

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>URI</th>
<th><a
href="http://www.w3.org/2004/02/skos/core#altLabel">http://www.w3.org/2004/02/skos/core#altLabel</a></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Foretrukken term</td>
<td></td>
</tr>
<tr class="even">
<td>Definition</td>
<td>En alternativ leksikalsk term for en ressource.</td>
</tr>
<tr class="odd">
<td>Kommentar</td>
<td><p>Range for skos:altLabel er klassen af RDF ’plain literals’.</p>
<p>skos:prefLabel, skos:altLabel og skos:hiddenLabel er parvis disjunkte
egenskaber.</p></td>
</tr>
<tr class="even">
<td>Eksempel</td>
<td>Akronymer, forkortelser, stavevarianter og uregelmæssige
flertals-/entalsformer kan inkluderes blandt de alternative betegnelser
for et begreb. Fejlstavede termer er normalt inkluderet som skjulte
etiketter (se skos:hiddenLabel).</td>
</tr>
<tr class="odd">
<td>Domæne</td>
<td>rdfs:Resource</td>
</tr>
<tr class="even">
<td>Udfaldsrum</td>
<td>xsd:string eller rdf:langString (tidligere angivet som
rdf:PlainLiteral)</td>
</tr>
<tr class="odd">
<td>Underegenskab af</td>
<td>rdfs:label</td>
</tr>
</tbody>
</table>

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-20}

<table>
<colgroup>
<col style="width: 22%" />
<col style="width: 77%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th>alternativ term</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Kommentar</td>
<td><p>[fra informationsmodel]</p>
<p>et andet navn for organisationen end det alment foretrukne.Ofte
opstår der alment kendte forkortelser eller alternative navne for
organisationer - især hvis det officielle navn er meget langt eller ikke
så mundret</p></td>
</tr>
<tr class="even">
<td>Anvendelsesnote</td>
<td>En alternativ leksikalsk term for en formel organisation. Bruges til
at angive et accepteret - men ikke foretrukkent - navn for
organisationen.</td>
</tr>
<tr class="odd">
<td>Eksempel</td>
<td><p>[fra informationsmodel]</p>
<p>navn: "Digitaliseringsstyrelsen"</p>
<p>alternativt navn: "Digst"</p>
<p>navn: "Styrelsen for dataforsyning og effektivisering"</p>
<p>alternativtNavn: "SDFE"</p></td>
</tr>
<tr class="even">
<td>Udfaldsrum</td>
<td>rdf:langString</td>
</tr>
<tr class="odd">
<td>Multiplicitet</td>
<td>0 - *</td>
</tr>
</tbody>
</table>

#### beskrivelse

##### *Vokabularets definition og beskrivelser*

| URI         | <http://purl.org/dc/terms/description>                                                                                                                        |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Term        | beskrivelse                                                                                                                                                   |
| Beskrivelse | Beskrivelsen kan omfatte, men er ikke begrænset til: et abstrakt, en indholdsfortegnelse, en grafisk repræsentation eller en fritekstberetning af ressourcen. |
| Kommentar   | En redegørelse for ressourcen.                                                                                                                                |
| Domæne      | rdfs:Resource                                                                                                                                                 |
| Udfaldsrum  | rdfs:Resource                                                                                                                                                 |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-21}

<table>
<colgroup>
<col style="width: 22%" />
<col style="width: 77%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th>beskrivelse</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Definition</td>
<td>En redegørelse for ressourcen.</td>
</tr>
<tr class="even">
<td>Beskrivelse</td>
<td><p>[fra informationsmodel]</p>
<p>letforståelig forklaring på organisationens virke.</p></td>
</tr>
<tr class="odd">
<td>Kommentar</td>
<td><p>[fra informationsmodel]</p>
<p>Beskrivelsen skal gerne formuleres således at den er forståelig af
andre end dem, der arbejder i organisationen, da formålet netop er at
udenforstående skal kunne få en vis indsigt i organisationens virke og
formål.</p></td>
</tr>
<tr class="even">
<td>Anvendelsesnote</td>
<td>Bruges til at angive en tekstbaseret beskrivelse af organisationens
formål og arbejde</td>
</tr>
<tr class="odd">
<td>Udfaldsrum</td>
<td>rdf:langString</td>
</tr>
<tr class="even">
<td>Multiplicitet</td>
<td>0 - *</td>
</tr>
</tbody>
</table>

#### p-nummer-reference

##### *Vokabularets definition og beskrivelser*

| URI             | https://data.gov.dk/model/core/orgextension/productionUnitCodeReference                                                                                                                                                                                                                                                                                                                                                                                    |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Term            | p-nummer-reference                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Definition      | reference til en associeret produktionsenhed i form af dennes p-nummer                                                                                                                                                                                                                                                                                                                                                                                     |
| Anvendelsesnote | Bruges til at angive et p-nummer, der er associeret med, men ikke formelt tilhører, den formelle organisation eller organisatoriske enhed. Et 'p-nummer' identificerer et sted, en lokation hvor en virksomhed har aktivitet. Ofte ses et p-nummer dog tilknyttet direkte til en instans af 'Formel organisation' eller 'Organisatorisk enhed', hvilket formelt set ikke er korrekt. For at håndtere denne brug er egenskaben 'p-nummer-reference' dannet. |
| Domæne          | rdfs:Resource                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Udfaldsrum      | xsd:string                                                                                                                                                                                                                                                                                                                                                                                                                                                 |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-22}

| Foretrukken term | p-nummer-reference                                                                             |
| ---------------- | ---------------------------------------------------------------------------------------------- |
| Definition       | En repræsentation af et produktionsenhedsnummer, anvendt som reference til produktionsenheden. |
| Domæne           | org:FormalOrganization                                                                         |
| Udfaldsrum       | xsd:string                                                                                     |
| Multiplicitet    | 0 - \*                                                                                         |

#### oprettelsesdato

##### *Vokabularets definition og beskrivelser*

| URI        | <http://schema.org/foundingDate>                  |
| ---------- | ------------------------------------------------- |
| Term       | grundlæggelsesdato                                |
| Kommentar  | Den dato, hvor denne organisation blev grundlagt. |
| Domæne     | schema:Organization                               |
| Udfaldsrum | schema:Date                                       |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-23}

| URI              | <http://schema.org/foundingDate>                                  |
| ---------------- | ----------------------------------------------------------------- |
| Foretrukken term | grundlæggelsesdato                                                |
| Alternativ term  | oprettelsesdato                                                   |
| Definition       | den dato organisationen blev grundlagt eller oprettet             |
| Anvendelsesnote  | Bruges til at angive den dato hvorpå organisationen blev oprettet |
| Kommentar        | Den dato, hvor denne organisation blev grundlagt.                 |
| Domæne           | org:FormalOrganization                                            |
| Udfaldsrum       | xsd:date                                                          |
| Multiplicitet    | 0 - 1                                                             |

#### nedlæggelsesdato

##### *Vokabularets definition og beskrivelser*

| URI        | <http://schema.org/dissolutionDate>        |
| ---------- | ------------------------------------------ |
| Term       | nedlæggelsesdato                           |
| Kommentar  | dato, hvor denne organisation blev opløst. |
| Domæne     | schema:Organization                        |
| Udfaldsrum | schema:Date                                |

##### 

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-24}

| Foretrukken term | nedlæggelsesdato                                                                                                    |
| ---------------- | ------------------------------------------------------------------------------------------------------------------- |
| Alternativ term  | Opløsningsdato                                                                                                      |
| Alternativ term  | ophørsdato                                                                                                          |
| Definition       | Den dato organisationen ophører med at eksistere.                                                                   |
| Kommentar        | Organisationen kan ikke ophøre med at eksistere så længe der er aktive Organisationsenheder eller -medlemmer i den. |
| Anvendelsesnote  | Bruges til at angive den dato hvorpå organisationen blev nedlagt                                                    |
| Domæne           | org:FormalOrganization                                                                                              |
| Udfaldsrum       | xsd:date                                                                                                            |
| Multiplicitet    | 0 - 1                                                                                                               |

## Eksempel på organisation

![](media/image18.emf)

##### JSON-LD-kode (uden context)

{

\"@id\" : \"xorg:org-844\",

\"@type\" : \"org:FormalOrganization\",

\"description\" : {

\"@language\" : \"da\",

\"@value\" : \"en kommune i Region Syddanmark\"

},

\"foundingDate\" : \"2007-01-01\",

\"label\" : \"org-844\",

\"prefLabel\" : {

\"@language\" : \"da\",

\"@value\" : \"Tønder Kommune\"

},

\"pUnitCodeReference\" : \"1003326862\",

}

## Typer af organisationer

![](media/image19.emf){width="6.211589020122485in"
height="1.7652176290463693in"}

Basisprofilen beskriver en organisations type med en klassifikation frem
for at oprette specialiseringer af organisationsklassen. Med andre ord
bliver organisationer af eksempelvis typen 'Offentlig myndighed' eller
'Interesseorganisation' beskrevet med brug af egenskaben
org:classification (klassifikation) til at angive typen af organisation,
frem for at oprette specialiseringer af org:FormalOrganization for hver
organisationstype.

Denne metode giver en mere fleksibel og hurtigere implementerbar måde at
inddrage nye organisationstyper på.

### Angivelse af en organisations type

![](media/image20.emf){width="5.35626968503937in"
height="0.7645833333333333in"}

#### klassifikation

##### *Vokabularets definition og beskrivelser*

| URI             | <http://www.w3.org/ns/org#classification>                                                                                                                                                                                                                    |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Term            | klassifikation                                                                                                                                                                                                                                               |
| Kommentar       | Angiver en klassifikation for denne organisation inden for et eller andet klassifikationssystem. Bemærk, at det også er tilladt for applikationer at definere underklasser af org:Organisation som et middel til at repræsentere organisatoriske kategorier. |
| Anvendelsesnote | udvidelsesvokabularer ønsker måske at specialisere denne egenskab til at have et område svarende til et specifikt skos:ConceptScheme                                                                                                                         |
| Domæne          | org:Organization                                                                                                                                                                                                                                             |
| Udfaldsrum      | skos:Concept                                                                                                                                                                                                                                                 |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-25}

| Definition      | Angiver en klassifikation for denne organisation inden for et eller andet klassifikationssystem. |
| --------------- | ------------------------------------------------------------------------------------------------ |
| Anvendelsesnote | Bruges her til at klassificere formelle organisationer                                           |
| Domæne          | org:FormalOrganization                                                                           |
| Udfaldsrum      | fot:FormalOrganizationType                                                                       |
| Multiplicitet   | 0 - \*                                                                                           |

### Typer af organisation (klasse)

![](media/image21.emf){width="2.548857174103237in"
height="0.7478269903762029in"}

##### *Vokabularets definition og beskrivelser*

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>URI</th>
<th>https://data.gov.dk/concept/core/formalorganizationtype/<br />
FormalOrganizationType</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Term</td>
<td>Type af organisation</td>
</tr>
<tr class="even">
<td>Definition</td>
<td>Klassifikation af formelle organisationer i forhold til
funktionsmæssige og juridiske type</td>
</tr>
<tr class="odd">
<td>Underklasse af</td>
<td>skos:Concept</td>
</tr>
</tbody>
</table>

#### **foretrukken betegnelse**

##### **Vokabularets definition og beskrivelser**

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>URI</th>
<th><a
href="http://www.w3.org/2004/02/skos/core#prefLabel">http://www.w3.org/2004/02/skos/core#prefLabel</a></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Term</td>
<td>foretrukken term</td>
</tr>
<tr class="even">
<td>Definition</td>
<td>Den foretrukne leksikalske betegnelse for en ressource på et givet
sprog.</td>
</tr>
<tr class="odd">
<td>Kommentar</td>
<td>En ressource har ikke mere end én værdi af skos:prefLabel pr.
sprogtag. Range for skos:prefLabel er klassen af RDF ’plain literals’.
skos:prefLabel, skos:altLabel, og skos:hiddenLabel er parvis disjunkte
egenskaber.</td>
</tr>
<tr class="even">
<td>Domæne</td>
<td>rdfs:Resource</td>
</tr>
<tr class="odd">
<td>Udfaldsrum</td>
<td><p>xsd:string eller rdf:langString</p>
<p>(tidligere angivet som rdf:PlainLiteral)</p></td>
</tr>
<tr class="even">
<td>Underegenskab af</td>
<td>rdfs:label</td>
</tr>
</tbody>
</table>

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-26}

| Foretrukken term | foretrukken term                                                          |
| ---------------- | ------------------------------------------------------------------------- |
| Definition       | Den foretrukne leksikalske betegnelse for en ressource på et givet sprog. |
| Domæne           | fot:FormalOrganizationType                                                |
| Udfaldsrum       | rdf:langString                                                            |
| Multiplicitet    | 1 - \*                                                                    |

#### alternativ betegnelse

##### *Vokabularets definition og beskrivelser*

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>URI</th>
<th><a
href="http://www.w3.org/2004/02/skos/core#altLabel">http://www.w3.org/2004/02/skos/core#altLabel</a></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Foretrukken term</td>
<td>alternativ term</td>
</tr>
<tr class="even">
<td>Definition</td>
<td>En alternativ leksikalsk term for en ressource.</td>
</tr>
<tr class="odd">
<td>Kommentar</td>
<td>Range for skos:altLabel er klassen af RDF ’plain literals’.
skos:prefLabel, skos:altLabel, og skos:hiddenLabel er parvis disjunkte
egenskaber. Akronymer, forkortelser, stavevarianter og uregelmæssige
flertals-/entalsformer kan inkluderes blandt de alternative betegnelser
for et begreb. Fejlstavede termer er normalt inkluderet som skjulte
etiketter (se skos:hiddenLabel).</td>
</tr>
<tr class="even">
<td>Eksempel</td>
<td>Akronymer, forkortelser, stavevarianter og uregelmæssige
flertals-/entalsformer kan inkluderes blandt de alternative betegnelser
for et begreb. Fejlstavede termer er normalt inkluderet som skjulte
etiketter (se skos:hiddenLabel).</td>
</tr>
<tr class="odd">
<td>Domæne</td>
<td>rdfs:Resource</td>
</tr>
<tr class="even">
<td>Udfaldsrum</td>
<td><p>xsd:string eller rdf:langString</p>
<p>(tidligere angivet som rdf:PlainLiteral)</p></td>
</tr>
<tr class="odd">
<td>Underegenskab af</td>
<td>rdfs:label</td>
</tr>
</tbody>
</table>

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-27}

| Foretrukken term | alternativ term                                 |
| ---------------- | ----------------------------------------------- |
| Definition       | En alternativ leksikalsk term for en ressource. |
| Domæne           | fot:FormalOrganizationType                      |
| Udfaldsrum       | rdf:langString                                  |
| Multiplicitet    | 0 - \*                                          |

#### definition

##### *Vokabularets definition og beskrivelser*

| URI              | <http://www.w3.org/2004/02/skos/core#definition>                  |
| ---------------- | ----------------------------------------------------------------- |
| Term             | definition                                                        |
| Definition       | En erklæring eller formel forklaring af betydningen af et begreb. |
| Underegenskab af | skos:note                                                         |
| Domæne           | rdfs:Resource                                                     |
| Udfaldsrum       | rdfs:Resource                                                     |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-28}

| Foretrukken term | definition                                                        |
| ---------------- | ----------------------------------------------------------------- |
| Definition       | En erklæring eller formel forklaring af betydningen af et begreb. |
| Domæne           | fot:FormalOrganizationType                                        |
| Udfaldsrum       | rdf:langString                                                    |
| Multiplicitet    | 0 - \*                                                            |

#### har bredere

##### *Vokabularets definition og beskrivelser*

| URI                   | <http://www.w3.org/2004/02/skos/core#broader>                                                                                                  |
| --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| Term                  |                                                                                                                                                |
| Definition            | Relaterer et begreb til et begreb, der har en mere generel betydning                                                                           |
| Kommentar             | Efter konvention bruges skos:broader kun til at erklære en umiddelbar (dvs. direkte) hierarkisk forbindelse mellem to konceptuelle ressourcer. |
| Underegenskab af      | skos:broaderTransitive                                                                                                                         |
| Modsatrettet egenskab | skos:narrower                                                                                                                                  |
| Domæne                | rdfs:Resource                                                                                                                                  |
| Udfaldsrum            | rdfs:Resource                                                                                                                                  |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-29}

| Foretrukken term | har bredere                                                          |
| ---------------- | -------------------------------------------------------------------- |
| Definition       | Relaterer et begreb til et begreb, der har en mere generel betydning |
| Domæne           | fot:FormalOrganizationType                                           |
| Udfaldsrum       | fot:FormalOrganizationType                                           |
| Multiplicitet    | 0 - 1                                                                |

## Eksempel på organisationstype

![](media/image22.emf)

##### JSON-LD-kode (uden context)

{

\"@id\" : \"xorg:org-844\",

\"@type\" : \"org:FormalOrganization\",

\"classification\" : \"fot:Municipality\",

}

##### fot:Municipality

{

\"@id\" : \"fot:Municipality\",

\"@type\" : \"fot:FormalOrganizationType\",

\"comment\" : {

\"@language\" : \"da\",

\"@value\" : \"Kommunen styres af en kommunalbestyrelse som bekendtgjort
i kommunebestyrelsesloven\"

},

\"label\" : \"Municipality\",

\"broader\" : \"fot:MunicipalAuthority\",

\"definition\" : \[ {

\"@language\" : \"da\",

\"@value\" : \"mindste offentlige forvaltningsenhed, der styres af en
kommunalbestyrelse som bekendtgjort i kommunebestyrelsesloven\"

}, {

\"@language\" : \"en\",

\"@value\" : \"smallest public administration unit that is governed by a
municipal council as promulgated in the Municipal Councils Act\"

} \],

\"prefLabel\" : \[ {

\"@language\" : \"da\",

\"@value\" : \"Kommune\"

}, {

\"@language\" : \"en\",

\"@value\" : \"Municipality\"

} \],

}

### Illustration

![](media/image23.emf)

Som indikeret i ovenstående illustration så benyttes egenskaben
org:classification til at udpege en klassifikation hvis emner
repræsenterer organisationstyper. I 'Bilag D -- Typer af organisation'
kan der findes uddybende beskrivelse af klassifikationen for
organisationer. Klassifikationen kan udvides løbende efter behov.

# Den organisatoriske enhed og dens egenskaber

![](media/image24.emf){width="6.608109142607174in"
height="3.0608694225721784in"}

## Organisatorisk enhed (klasse)

![](media/image25.emf){width="2.234782370953631in"
height="0.7993055555555556in"}

##### *Vokabularets definition og beskrivelser*

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>URI</th>
<th><a
href="http://www.w3.org/ns/org#OrganizationalUnit">http://www.w3.org/ns/org#OrganizationalUnit</a></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Term</td>
<td>Organisatorisk enhed</td>
</tr>
<tr class="even">
<td>Kommentar</td>
<td>En organisation, såsom en afdeling eller supportenhed, som er en del
af en større organisation og kun har fuld anerkendelse inden for den
pågældende organisations kontekst. Navnlig vil enheden ikke blive
betragtet som en juridisk enhed i sig selv.</td>
</tr>
<tr class="odd">
<td>Anvendelsesnote</td>
<td>Enheder kan være store og komplekse og indeholde andre enheder.
Alternative navne: Afdeling</td>
</tr>
<tr class="even">
<td>Underklasse af</td>
<td><p>foaf:Organization</p>
<p>org:Organization</p></td>
</tr>
</tbody>
</table>

##### 

##### Profilens restriktioner og beskrivelser {#profilens-restriktioner-og-beskrivelser-30}

<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 79%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th>Organisatorisk enhed</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Alternativ term</td>
<td>Afdeling; sektion; kontor; team; udvalg</td>
</tr>
<tr class="even">
<td>Definition</td>
<td>En organisation, såsom en afdeling eller supportenhed, som er en del
af en større organisation og kun har fuld anerkendelse inden for den
pågældende organisations kontekst. Navnlig vil enheden ikke blive
betragtet som en juridisk enhed i sig selv.</td>
</tr>
<tr class="odd">
<td>Kommentar</td>
<td><p>organisationsenheder kan være mere eller mindre permanente.
Eksempelvis kan der oprettes en organisationsenhed til et projekt,
hvorefter den opløses, når projektet er slut. Eller en
organisationsenhed kan være en permanent del af organisationen, som
f.eks. "bogholderiet".</p>
<p>Fælles for organisationsenheder er, at de har til formål at have
noget at samle organisationsmedlemmer i og kan omtale som noget kendt i
organisationen.</p></td>
</tr>
<tr class="even">
<td>Eksempel</td>
<td><p>[Fra informationsmodel]</p>
<p>Bogholderiet</p>
<p>Projekt "ny organisationsstandard"</p>
<p>Hæmatologisk afdeling</p>
<p>....</p></td>
</tr>
</tbody>
</table>

## Den organisatoriske enheds egenskaber

Den organisatoriske enheds brug af egenskaben adms:identifier og klassen
adms:Identifier dækkes af beskrivelsen i afsnittet 'Beskrivelse af
klasse og egenskaber til identifikation'

#### foretrukken betegnelse

##### *Vokabularets definition og beskrivelser*

| URI              | <http://www.w3.org/2004/02/skos/core#prefLabel>                                                                                                                                                                         |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Term             | foretrukken term                                                                                                                                                                                                        |
| Foretrukken term | Den foretrukne leksikalske betegnelse for en ressource på et givet sprog.                                                                                                                                               |
| Kommentar        | En ressource har ikke mere end én værdi af skos:prefLabel pr. sprogtag. Range for skos:prefLabel er klassen af RDF 'plain literals'. skos:prefLabel, skos:altLabel, og skos:hiddenLabel er parvis disjunkte egenskaber. |
| Underegenskab af | rdfs:label                                                                                                                                                                                                              |
| Domæne           | rdfs:Resource                                                                                                                                                                                                           |
| Udfaldsrum       | xsd:string eller rdf:langString (tidligere angivet som rdf:PlainLiteral)                                                                                                                                                |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-31}

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>alternative term</th>
<th>enhedsnavn</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Alternativ term</td>
<td>afdelingsnavn</td>
</tr>
<tr class="even">
<td>Definition</td>
<td>alment anvendt navn for en organisationsenhed</td>
</tr>
<tr class="odd">
<td>Kommentar</td>
<td>Alment anvendt navn for en organisationsenhed, der normalt tildeles
af organisationen</td>
</tr>
<tr class="even">
<td>Anvendelsesnote</td>
<td>Bruges til at angive den organisatoriske enheds primære navn.</td>
</tr>
<tr class="odd">
<td>Eksempel</td>
<td><p>"Bogholderiet"</p>
<p>Projekt "ny organisationsstandard"</p>
<p>"Hæmatologisk afdeling"</p>
<p>...</p></td>
</tr>
<tr class="even">
<td>Domæne</td>
<td>org:OrganizationalUnit</td>
</tr>
<tr class="odd">
<td>Udfaldsrum</td>
<td>rdf:langString</td>
</tr>
<tr class="even">
<td>Multiplicitet</td>
<td>1 - *</td>
</tr>
</tbody>
</table>

#### alternativ betegnelse

##### *Vokabularets definition og beskrivelser*

| URI              | <http://www.w3.org/2004/02/skos/core#altLabel>                                                                                                                                                                                        |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Foretrukken term | alternativ term                                                                                                                                                                                                                       |
| Definition       | En alternativ leksikalsk term for en ressource.                                                                                                                                                                                       |
| Kommentar        | Range for skos:altLabel er klassen af RDF \'plain literals\'. skos:prefLabel, skos:altLabel, og skos:hiddenLabel er parvis disjunkte egenskaber.                                                                                      |
| Eksempel         | Akronymer, forkortelser, stavevarianter og uregelmæssige flertals-/entalsformer kan inkluderes blandt de alternative betegnelser for et begreb. Fejlstavede termer er normalt inkluderet som skjulte etiketter (se skos:hiddenLabel). |
| Underegenskab af | rdfs:label                                                                                                                                                                                                                            |
| Domæne           | rdfs:Resource                                                                                                                                                                                                                         |
| Udfaldsrum       | xsd:string eller rdf:langString (tidligere angivet som rdf:PlainLiteral)                                                                                                                                                              |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-32}

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th>alternativ term</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Kommentar</td>
<td>Ofte opstår der alment kendte forkortelser eller alternative navne
for organisationsenheder - især hvis det officielle navn er meget langt
eller ikke så mundret.</td>
</tr>
<tr class="even">
<td>Anvendelsesnote</td>
<td>Bruges til at angive et accepteret - men ikke foretrukket - navn for
den organisatoriske enhed.</td>
</tr>
<tr class="odd">
<td>Eksempel</td>
<td><p>navn: "Digitalisering og Arkitektur"</p>
<p>alternativt navn: "DIA"</p>
<p>navn: Kontor for Offentligret</p>
<p>alternativt navn: Jura</p></td>
</tr>
<tr class="even">
<td>Udfaldsrum</td>
<td>rdf:langString</td>
</tr>
<tr class="odd">
<td>Multiplicitet</td>
<td>0 - *</td>
</tr>
</tbody>
</table>

#### beskrivelse  {#beskrivelse-1}

##### *Vokabularets definition og beskrivelser*

| URI         | <http://purl.org/dc/terms/description>                                                                                                                        |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Term        | beskrivelse                                                                                                                                                   |
| Beskrivelse | Beskrivelsen kan omfatte, men er ikke begrænset til: et abstrakt, en indholdsfortegnelse, en grafisk repræsentation eller en fritekstberetning af ressourcen. |
| Kommentar   | En redegørelse for ressourcen.                                                                                                                                |
| Domæne      | rdfs:Resource                                                                                                                                                 |
| Udfaldsrum  | rdfs:Resource                                                                                                                                                 |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-33}

<table>
<colgroup>
<col style="width: 22%" />
<col style="width: 77%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th>beskrivelse</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Anvendelsesnote</td>
<td>letforståelig forklaring på organisationsenhedens virke og
formål.</td>
</tr>
<tr class="even">
<td>Kommentar</td>
<td><p>[fra informationsmodel]</p>
<p>Beskrivelsen skal gerne formuleres således at den er forståelig af
andre end dem, der arbejder i organisationsenheden, da formålet netop er
at udenforstående skal kunne få en vis indsigt i organisationsenhedens
virke og formål.</p></td>
</tr>
<tr class="odd">
<td>Anvendelsesnote</td>
<td>Bruges til at angive en tekstbaseret beskrivelse af
organisationsenhedens formål og arbejde</td>
</tr>
<tr class="even">
<td>Udfaldsrum</td>
<td>rdf:langString</td>
</tr>
<tr class="odd">
<td>Multiplicitet</td>
<td>0 - *</td>
</tr>
</tbody>
</table>

#### oprettelsesdato

##### *Vokabularets definition og beskrivelser*

| URI             | <http://schema.org/foundingDate>      |
| --------------- | ------------------------------------- |
| Term            | grundlæggelsesdato                    |
| Alternativ term | oprettelsesdato                       |
| Kommentar       | den dato organisationen blev oprettet |
| Domæne          | schema:Organization                   |
| Udfaldsrum      | schema:Date                           |

##### *Profilens restriktioner og beskrivelser* {#profilens-restriktioner-og-beskrivelser-34}

| Foretrukken term | grundlæggelsesdato                                                                                                                                                                                  |
| ---------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Anvendelsesnote  | Anvendt i denne sammenhæng angiver egenskaben den dato hvorpå den organisatoriske enhed blev oprettet. I schema.org anvendes termen 'organisation' bredt og dækker også over 'organisatorisk enhed' |
| Domæne           | org:OrganizationalUnit                                                                                                                                                                              |
| Udfaldsrum       | xsd:date                                                                                                                                                                                            |
| Multiplicitet    | 0 - 1                                                                                                                                                                                               |

#### nedlæggelsesdato

##### *Vokabularets definition og beskrivelser*

| URI        | <http://schema.org/dissolutionDate>  |
| ---------- | ------------------------------------ |
| Term       | nedlæggelsesdato                     |
| Kommentar  | den dato organisationen blev nedlagt |
| Domæne     | schema:Organization                  |
| Udfaldsrum | schema:Date                          |

##### Profilens restriktioner og beskrivelser {#profilens-restriktioner-og-beskrivelser-35}

| Foretrukken term | nedlæggelsesdato                                                                                                                                                                          |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Alternativ term  | opløsningsdato                                                                                                                                                                            |
| Kommentar        | nedlæggelsesdatoen skal være lig med eller senere end oprettelsesdatoen                                                                                                                   |
| Anvendelsesnote  | . Anvendt i denne sammenhæng angiver den dato hvorpå den organisatoriske enhed blev nedlagt. I schema.org anvendes termen 'organisation' bredt og dækker også over 'organisatorisk enhed' |
| Domæne           | org:OrganizationalUnit                                                                                                                                                                    |
| Udfaldsrum       | xsd:date                                                                                                                                                                                  |
| Multiplicitet    | 0 - 1                                                                                                                                                                                     |

#### p-nummer-reference

Et 'p-nummer' identificerer et sted, en lokation hvor en virksomhed har
aktivitet. Ofte ses et p-nummer dog tilknyttet direkte til en instans af
'Formel organisation' eller 'Organisatorisk enhed', hvilket formelt set
ikke er korrekt. For at håndtere denne brug er egenskaben
'p-nummer-reference' dannet.

##### *Vokabularets definition og beskrivelser*

| URI        | https://data.gov.dk/model/core/orgextension/productionUnitCodeReference                       |
| ---------- | --------------------------------------------------------------------------------------------- |
| Term       | p-nummer-reference                                                                            |
| Definition | En repræsentation af et produktionsenhedsnummer, anvendt som reference til produktionsenheden |
| Domæne     | rdfs:Resource                                                                                 |
| Udfaldsrum | xsd:string                                                                                    |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-36}

| Foretrukken term | p-nummer-reference     |
| ---------------- | ---------------------- |
| Domæne           | org:OrganizationalUnit |
| Udfaldsrum       | xsd:string             |
| Multiplicitet    | 0 - \*                 |

## Typer af organisatoriske enheder

![](media/image26.emf){width="6.54700678040245in"
height="1.6956517935258093in"}

Basisprofilen beskriver en organisatorisk enheds type med en
klassifikation frem for at oprette specialiseringer af den
organisatoriske enheds klasse. Organisatoriske enheder som 'afdeling' og
team' beskrives med brug af egenskaben org:classification
(klassifikation) til at angive enhedstypen, frem for at oprette
specialiseringer af org:OrganizationalUnit for hver enhedstype.

Denne metode giver en mere fleksibel og hurtigere implementerbar måde at
inddrage nye enhedstyper på.

### Angivelse af typen af organisatorisk enhed

![](media/image27.emf){width="5.526802274715661in"
height="0.8173906386701663in"}

#### klassifikation

##### *Vokabularets definition og beskrivelser*

| URI        | <http://www.w3.org/ns/org#classification>                                                                                                                                                                                                                                                                                                                                                                                    |
| ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Term       | klassifikation                                                                                                                                                                                                                                                                                                                                                                                                               |
| Kommentar  | Angiver en klassifikation for denne Organisation inden for et klassifikationsskema. Udvidelsesvokabularer ønsker måske at specialisere denne egenskab til at have et område svarende til et specifikt \'skos:ConceptScheme\'. Denne egenskab er under diskussion og kan blive revideret eller fjernet - i mange tilfælde kategoriseres organisationer bedst ved at definere et underklassehierarki i et udvidelsesvokabular. |
| Domæne     | org:Organization                                                                                                                                                                                                                                                                                                                                                                                                             |
| Udfaldsrum | skos:Concept                                                                                                                                                                                                                                                                                                                                                                                                                 |

##### *Profilens restriktioner og beskrivelser* {#profilens-restriktioner-og-beskrivelser-37}

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th>klassifikation</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Definition</td>
<td>Angiver en klassifikation for denne Organisationinden for et
klassifikationssystem.</td>
</tr>
<tr class="even">
<td>Anvendelsesnote</td>
<td>Beskriver den slags organisationsenhed der er tale om. I schema.org
anvendes termen ’organisation’ bredt og dækker også over ’organisatorisk
enhed’</td>
</tr>
<tr class="odd">
<td>Kommentar</td>
<td><p>[fra informationsmodel]</p>
<p>Kan anvendes til at imødekomme forskellige forretningsregler, som
retter sig mod typen af Organisationsenhed.</p></td>
</tr>
<tr class="even">
<td>Eksempel</td>
<td><p>[fra informationsmodel]</p>
<ul>
<li><blockquote>
<p>klinisk-administrativt niveau</p>
</blockquote></li>
<li><blockquote>
<p>økonomi</p>
</blockquote></li>
<li><blockquote>
<p>...</p>
</blockquote></li>
</ul></td>
</tr>
<tr class="odd">
<td>Domæne</td>
<td>org:OrganizationalUnit</td>
</tr>
<tr class="even">
<td>Udfaldsrum</td>
<td>out:OrganizationalUnitType</td>
</tr>
<tr class="odd">
<td>Multiplicitet</td>
<td>0 - *</td>
</tr>
</tbody>
</table>

### Klassen Organisatorisk enhedstype

![](media/image28.emf){width="3.156313429571304in"
height="1.7043471128608925in"}

##### *Vokabularets definition og beskrivelser*

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>URI</th>
<th>https://data.gov.dk/concept/core/organisationalunittype/<br />
OrganizationalUnitType</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Term</td>
<td>Organisatoriske enhedstype</td>
</tr>
<tr class="even">
<td>Foretrukken term</td>
<td>Organisatoriske enhedstype</td>
</tr>
<tr class="odd">
<td>Definition</td>
<td>Klassifikation af organisationstyper</td>
</tr>
<tr class="even">
<td>Underklasse af</td>
<td>skos:Concept</td>
</tr>
</tbody>
</table>

#### foretrukken term

##### *Vokabularets definition og beskrivelser*

| URI              | <http://www.w3.org/2004/02/skos/core#prefLabel>                                                                                                                                                                        |
| ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Term             | foretrukken term                                                                                                                                                                                                       |
| Definition       | Den foretrukne leksikalske betegnelse for en ressource på et givet sprog.                                                                                                                                              |
| Kommentar        | En ressource har ikke mere end én værdi af skos:prefLabel pr. sprogtag. Range for skos:prefLabel er klassen af RDF 'plain literals'. skos:prefLabel, skos:altLabel og skos:hiddenLabel er parvis disjunkte egenskaber. |
| Underegenskab af | rdfs:label                                                                                                                                                                                                             |
| Domæne           | rdfs:Resource                                                                                                                                                                                                          |
| Udfaldsrum       | xsd:string eller rdf:langString (tidligere angivet som rdf:PlainLiteral)                                                                                                                                               |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-38}

| Foretrukken term | foretrukken term                                                                   |
| ---------------- | ---------------------------------------------------------------------------------- |
| Anvendelsesnote  | Den foretrukne leksikalske betegnelse for en organisationstypen på et givet sprog. |
| Anvendelsesnote  | Bruges til at angive den organisatoriske enhedstypes foretrukne navn.              |
| Domæne           | rdfs:Resource                                                                      |
| Udfaldsrum       | rdf:langString                                                                     |
| Multiplicitet    | 1 - \*                                                                             |

#### alternativ term

##### *Vokabularets definition og beskrivelser*

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>URI</th>
<th><a
href="http://www.w3.org/2004/02/skos/core#altLabel">http://www.w3.org/2004/02/skos/core#altLabel</a></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Foretrukken term</td>
<td>alternativ term</td>
</tr>
<tr class="even">
<td>Definition</td>
<td>En alternativ leksikalsk term for en ressource.</td>
</tr>
<tr class="odd">
<td>Kommentar</td>
<td>Range for skos:altLabel er klassen af RDF ’plain literals’.
skos:prefLabel, skos:altLabel og skos:hiddenLabel er parvis disjunkte
egenskaber. Akronymer, forkortelser, stavevarianter og uregelmæssige
flertals-/entalsformer kan inkluderes blandt de alternative betegnelser
for et begreb. Fejlstavede termer er normalt inkluderet som skjulte
etiketter (se skos:hiddenLabel).</td>
</tr>
<tr class="even">
<td>Eksempel</td>
<td>Akronymer, forkortelser, stavevarianter og uregelmæssige
flertals-/entalsformer</td>
</tr>
<tr class="odd">
<td>Underegenskab af</td>
<td>rdfs:label</td>
</tr>
<tr class="even">
<td>Domæne</td>
<td>rdfs:Resource</td>
</tr>
<tr class="odd">
<td>Udfaldsrum</td>
<td><p>xsd:string eller rdf:langString</p>
<p>(tidligere angivet som rdf:PlainLiteral)</p></td>
</tr>
</tbody>
</table>

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-39}

| Foretrukken term | alternativ term                                                                                      |
| ---------------- | ---------------------------------------------------------------------------------------------------- |
| Definition       | En alternativ leksikalsk term for den organisatoriske enhedstype                                     |
| Anvendelsesnote  | Bruges til at angive et accepteret - men ikke foretrukkent - navn for den organisatoriske enhedtype. |
| Domæne           | rdfs:Resource                                                                                        |
| Udfaldsrum       | rdf:langString                                                                                       |
| Multiplicitet    | 0 - \*                                                                                               |

#### definition

##### *Vokabularets definition og beskrivelser*

| URI              | <http://www.w3.org/2004/02/skos/core#definition>                  |
| ---------------- | ----------------------------------------------------------------- |
| Term             | definition                                                        |
| Definition       | En erklæring eller formel forklaring af betydningen af et begreb. |
| Underegenskab af | skos:note                                                         |
| Domæne           | rdfs:Resource                                                     |
| Udfaldsrum       | rdfs:Resource                                                     |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-40}

| Foretrukken term | definition                                                        |
| ---------------- | ----------------------------------------------------------------- |
| Definition       | En erklæring eller formel forklaring af betydningen af et begreb. |
| Domæne           | out:OrganizationalUnitType                                        |
| Udfaldsrum       | rdf:langString                                                    |
| Multiplicitet    | 0 - \*                                                            |

#### har bredere

##### *Vokabularets definition og beskrivelser*

| URI                   | <http://www.w3.org/2004/02/skos/core#broader>                                                                                                  |
| --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| Term                  | har bredere                                                                                                                                    |
| Definition            | Relaterer et begreb til et begreb, der har en mere generel betydning                                                                           |
| Kommentar             | Efter konvention bruges skos:broader kun til at erklære en umiddelbar (dvs. direkte) hierarkisk forbindelse mellem to konceptuelle ressourcer. |
| Underegenskab af      | skos:broaderTransitive                                                                                                                         |
| Modsatrettet egenskab | skos:narrower                                                                                                                                  |
| Domæne                | rdfs:Resource                                                                                                                                  |
| Udfaldsrum            | rdfs:Resource                                                                                                                                  |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-41}

| Foretrukken term | har bredere                                                          |
| ---------------- | -------------------------------------------------------------------- |
| Definition       | Relaterer et begreb til et begreb, der har en mere generel betydning |
| Domæne           | out:OrganizationalUnitType                                           |
| Udfaldsrum       | out:OrganizationalUnitType                                           |
| Multiplicitet    | 0 - 1                                                                |

### Illustration af typer

![](media/image29.emf)

I 'Bilag E -- Typer af organisatoriske enheder' beskrives typerne for
organisationenheder yderligere.

# Kvalificeret kontaktinformation

En organisation kan kontaktes af eksterne på forskellige måder.
Kontakten kan ske ved personligt fremmøde til en besøgsadresse eller ved
at sende post til postadresse. Kontakten kan også foretages via telefon,
fax, e-mail eller en dedikeret webside.

I basisprofilen er alle de nævnte kontaktformer repræsenteret både i
relation til den formelle organisation og i relation til organisatoriske
enheder.

Kontaktformerne er repræsenteret som kvalificeret information.
Kvalificeret information betyder i denne sammenhæng at der til
kontaktformen, eksempelvis et telefonnummer, tilføjes data der giver
mere information, eksempelvis hvilke tidspunkter der kan ringes på.

![](media/image30.emf){width="6.679044181977253in"
height="4.0869564741907265in"}

### kontaktpunkt

##### Vokabularets definition og beskrivelser

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 74%" />
</colgroup>
<thead>
<tr class="header">
<th>URI</th>
<th><a
href="https://schema.org/contactPoint">https://schema.org/contactPoint</a></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Term</td>
<td>kontaktpunkt</td>
</tr>
<tr class="even">
<td>Kommentar</td>
<td><blockquote>
<p>Et kontaktpunkt for en person eller organisation.</p>
</blockquote></td>
</tr>
<tr class="odd">
<td>Domæne inkluderer</td>
<td>schema:Organization eller schema:Person eller
schema:HealthInsurancePlan</td>
</tr>
<tr class="even">
<td>Udfaldsrum inkluderer</td>
<td>schema:ContactPoint eller schema:Text eller schema:URL eller
schema:Role</td>
</tr>
</tbody>
</table>

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-42}

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 74%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th><blockquote>
<p>kontaktpunkt</p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Definition</td>
<td><blockquote>
<p>Et kontaktpunkt for en formel organisation eller en organisatorisk
enhed.</p>
</blockquote></td>
</tr>
<tr class="even">
<td>Domæne</td>
<td><blockquote>
<p>org:FormalOrganization eller org:OrganizationalUnit</p>
</blockquote></td>
</tr>
<tr class="odd">
<td>Udfaldsrum</td>
<td><blockquote>
<p>schema:ContactPoint</p>
</blockquote></td>
</tr>
<tr class="even">
<td>Multiplicitet</td>
<td>0 - *</td>
</tr>
</tbody>
</table>

### Klassen Kontaktpunkt

Instanser af klassen schema:ContactPoint bruges til at give uddybende
('kvalificeret') information om en måde hvorpå organisationen eller en
af dens enheder kan kontaktes.

Instansen skal altid have oplysning om kontaktformen via
klassifikationsklassen ci:ContactMethodType.

Den egentlige kontaktinformation -- eksempelvis telefon eller e-mail --
angives ved brug af dcterms:identifier.

Hvis kontaktmuligheden er dedikeret specifikke emner eller formål kan
disse angives ved brug af schema:contactType.

Hvis der er særlige tidspunkter for brugen af kontaktformen kan disse
angives via schema:OpeningHoursSpecification.

![](media/image31.emf){width="4.260869422572179in"
height="2.7412193788276467in"}

#### Kontaktpunkt

##### *Vokabularets definition og beskrivelser*

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 74%" />
</colgroup>
<thead>
<tr class="header">
<th>URI</th>
<th>https://schema.org/ContactPoint</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Term</td>
<td><blockquote>
<p>Kontaktpunkt</p>
</blockquote></td>
</tr>
<tr class="even">
<td>Kommentar</td>
<td><blockquote>
<p>Et kontaktpunkt, f.eks. en kundeklageafdeling</p>
</blockquote></td>
</tr>
<tr class="odd">
<td>Underklasse af</td>
<td>schema:StructuredValue</td>
</tr>
</tbody>
</table>

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-43}

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 74%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th>Kontaktpunkt</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Definition</td>
<td>Information om kontaktmetode samt hvilke muligheder og begrænsninger
der er ved brug af den pågældende kontaktmetode.</td>
</tr>
<tr class="even">
<td>Kommentar</td>
<td><blockquote>
<p>[fra informationsmodel (klassen Kontaktinformation)]</p>
<p>Kan omhandle fysiske steder som adresser, lokaler, men også virtuelle
som sociale medier, email, DigitalPost mv.</p>
</blockquote></td>
</tr>
<tr class="odd">
<td>Eksempel</td>
<td><blockquote>
<p>[fra informationsmodel (klassen Kontaktinformation)]</p>
<p>- fysisk adresse</p>
<p>- elektronisk adresse</p>
<p>- email</p>
</blockquote></td>
</tr>
</tbody>
</table>

#### identifikator

##### *Vokabularets definition og beskrivelser*

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 74%" />
</colgroup>
<thead>
<tr class="header">
<th>URI</th>
<th><blockquote>
<p>http://purl.org/dc/terms/identifier</p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Term</td>
<td><blockquote>
<p>identifikator</p>
</blockquote></td>
</tr>
<tr class="even">
<td>Beskrivelse</td>
<td>Anbefalet bedste praksis er at identificere ressourcen ved hjælp af
en streng, der er i overensstemmelse med et formelt
identifikationssystem.</td>
</tr>
<tr class="odd">
<td>Kommentar</td>
<td><blockquote>
<p>En entydig reference til ressourcen inden for en given kontekst.</p>
</blockquote></td>
</tr>
<tr class="even">
<td>Domæne</td>
<td><blockquote>
<p>rdfs:Resource</p>
</blockquote></td>
</tr>
<tr class="odd">
<td>Udfaldsrum</td>
<td><blockquote>
<p>rdfs:Literal</p>
</blockquote></td>
</tr>
</tbody>
</table>

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-44}

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 74%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th><blockquote>
<p>identifikator</p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Definition</td>
<td>Det konkrete indhold for den specifikke kontaktform
kontaktinformationen har.</td>
</tr>
<tr class="even">
<td>Eksempel</td>
<td><blockquote>
<p>Eksempler på værdier udtrykt ved brug af de nævnte standarder og
retningslinjer:</p>
<p>Statsministeriets telefonnummeret: +4533923300</p>
<p>Statsministeriets mailadresse: stm@stm.dk .</p>
<p>Statsministeriets webadresse: <a
href="https://www.stm.dk/">https://www.stm.dk/</a></p>
<p>Statsministeriets adresse: Prins Jørgens Gård 11, 1218 København
K</p>
</blockquote></td>
</tr>
<tr class="odd">
<td>Domæne</td>
<td><blockquote>
<p>schema:ContactPoint</p>
</blockquote></td>
</tr>
<tr class="even">
<td>Udfaldsrum</td>
<td><blockquote>
<p>xsd:string</p>
</blockquote></td>
</tr>
<tr class="odd">
<td>Multiplicitet</td>
<td><blockquote>
<p>1 - 1</p>
</blockquote></td>
</tr>
</tbody>
</table>

#### kontaktformål

##### *Vokabularets definition og beskrivelser*

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 74%" />
</colgroup>
<thead>
<tr class="header">
<th>URI</th>
<th>https://schema.org/contactType</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Term</td>
<td>kontaktype</td>
</tr>
<tr class="even">
<td>Kommentar</td>
<td>En person eller organisation kan have forskellige kontaktpunkter til
forskellige formål. For eksempel et salgskontaktpunkt, et
PR-kontaktpunkt og så videre. Denne egenskab bruges til at angive typen
af kontaktpunkt.</td>
</tr>
<tr class="odd">
<td>Domæne inkluderer</td>
<td>schema:ContactPoint</td>
</tr>
<tr class="even">
<td>Udfaldsrum inkluderer</td>
<td><p>schema:Text</p>
<p>or schema:URL</p>
<p>or schema:Role</p></td>
</tr>
</tbody>
</table>

##### *Profilens restriktioner og beskrivelser* {#profilens-restriktioner-og-beskrivelser-45}

| Foretrukken term | kontakformål                               |
| ---------------- | ------------------------------------------ |
| Definition       | Angiver det specifikke kontaktpunktsformål |
| Domæne           | schema:ContactPoint                        |
| Udfaldsrum       | rdf:langString                             |
| Multiplicitet    | 0 - 1                                      |

#### kommentar

##### *Vokabularets definition og beskrivelser*

| URI       | <http://www.w3.org/1999/02/22-rdf-syntax-ns#comment> |
| --------- | ---------------------------------------------------- |
| Term      | kommentar                                            |
| Kommentar | En beskrivelse af den pågældenderessource.           |

##### *Profilens restriktioner og beskrivelser* {#profilens-restriktioner-og-beskrivelser-46}

<table>
<colgroup>
<col style="width: 28%" />
<col style="width: 71%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th>kommentar</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Definition</td>
<td>en beskrivelse af den pågældende ressource</td>
</tr>
<tr class="even">
<td>Anvendelsesnote</td>
<td><p>[fra informationsmodel (klassen Kontaktinformation)]</p>
<p>anvendes til at beskrive regler og principper for anvendelse af den
enkelte kontaktform</p></td>
</tr>
<tr class="odd">
<td>Kommentar</td>
<td><p>[fra informationsmodel (klassen Kontaktinformation)]</p>
<p>Giver mulighed for at angive særlige forhold, afvigelser eller andet
relevant information der knytter sig til den enkelte
kontakttype.</p></td>
</tr>
<tr class="even">
<td>Kommentar</td>
<td><p>[fra informationsmodel (klassen Kontaktinformation)]</p>
<p>Der kan være regler/principper som gælder for samtlige kontakttyper,
men der kan også være særlige politikker der kun gør sig gældende i
forhold til en specifik kontakttype.</p></td>
</tr>
<tr class="odd">
<td>Eksempel</td>
<td><p>[fra informationsmodel (klassen Kontaktinformation)]</p>
<p>Benyt indgangen i parkeringskælderen</p></td>
</tr>
<tr class="even">
<td>Eksempel</td>
<td><p>[fra informationsmodel (klassen Kontaktinformation)]</p>
<p>- email besvares inden for 5 hverdage.</p></td>
</tr>
<tr class="odd">
<td>Udfaldsrum</td>
<td>rdf:langString</td>
</tr>
<tr class="even">
<td>Multiplicitet</td>
<td>0 - *</td>
</tr>
</tbody>
</table>

#### type

##### *Vokabularets definition og beskrivelser*

| URI         | http://purl.org/dc/terms/type                                                                                                                                                                                    |
| ----------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Term        | type                                                                                                                                                                                                             |
| Beskrivelse | Anbefalet bedste praksis er at bruge et kontrolleret ordforråd, såsom DCMI Type Vocabulary \[DCMITYPE\]. For at beskrive ressourcens filformat, fysiske medium eller dimensioner skal du bruge Format-elementet. |
| Kommentar   | Ressourcens art eller genre.                                                                                                                                                                                     |
| Domæne      | rdfs:Resource                                                                                                                                                                                                    |
| Udfaldsrum  | rdfs:Class                                                                                                                                                                                                       |

##### *Profilens restriktioner og beskrivelser* {#profilens-restriktioner-og-beskrivelser-47}

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th>type</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Definition</td>
<td><blockquote>
<p>ressourcens art eller genre</p>
</blockquote></td>
</tr>
<tr class="even">
<td>Alternativ term</td>
<td></td>
</tr>
<tr class="odd">
<td>anvendelsesnote</td>
<td><p>[fra informationsmodel (klassen Kontaktinformation)]</p>
<p>anvendes til at klassificere de forskellige typer af
kontaktpunkter</p></td>
</tr>
<tr class="even">
<td>Kommentar</td>
<td><p>[fra informationsmodel (klassen Kontaktinformation)]</p>
<p>omhandler fx fysiske steder som adresser, lokaler, men også virtuelle
som sociale medier, email, DigitalPost mv.</p></td>
</tr>
<tr class="odd">
<td>Anvendelsesnote</td>
<td>Udpeger typen af kontaktform</td>
</tr>
<tr class="even">
<td>Domæne</td>
<td>schema:ContactPoint</td>
</tr>
<tr class="odd">
<td>Udfaldsrum</td>
<td>ci:ContactFormType</td>
</tr>
<tr class="even">
<td>Multiplicitet</td>
<td>1 - 1</td>
</tr>
</tbody>
</table>

### Type af kontaktmetode (klasse)

![](media/image32.emf){width="3.904348206474191in"
height="1.6552001312335958in"}

##### *Vokabularets definition og beskrivelser*

| URI            | https://data.gov.dk/concept/core/contactinformation/ContactMethodType |
| -------------- | --------------------------------------------------------------------- |
| Term           | Type af kontaktform                                                   |
| Definition     | Klassifikationsklasse indeholdende mulige kontaktformer.              |
| Underklasse af | skos:Concept                                                          |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-48}

| Foretrukken term | Kontaktform                                                                                                                                                                                                                                                                                                                                                                          |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Definition       | Klassifikationsklasse indeholdende mulige kontaktformer                                                                                                                                                                                                                                                                                                                              |
| Definition       | anvendes til at klassificere de forskellige typer af kontaktpunkter                                                                                                                                                                                                                                                                                                                  |
| Kommentar        | Kontaktform vil - af den nedsatte redaktionsgruppe - blive vedligeholdt kontinuerligt. Som en del af det arbejde vil koordinering med eksisterende, kendte og aktivt anvendte registres beskrivelse af kontaktformer blive anvendt som input til basisprofilens kontaktformer. Basisprofilens kontaktformer skal kunne dække alle relevante kontaktformer fra og til organisationer. |

I 'Bilag F -- Type af kontaktmetode' beskrives de enkelte kontaktmetoder
i detaljer.

### Specifikation af åbningstider

![](media/image33.emf){width="3.262589676290464in"
height="5.034782370953631in"}

#### timer tilgængelige

##### *Vokabularets definition og beskrivelser*

| URI               | https://schema.org/hoursAvailable                                                     |
| ----------------- | ------------------------------------------------------------------------------------- |
| Term              | åbningstid (eller evt. tilgængeligt tidsrum)                                          |
| Kommentar         | De timer, hvor denne service eller kontakt er tilgængelig.                            |
| Domæne inkluderer | schema:LocationFeatureSpecification eller schema:ContactPoint eller schema:Service    |
| Udfaldsrum        | schema:OpeningHoursSpecification eller schema:Text eller schema:URL eller schema:Role |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-49}

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 74%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th><blockquote>
<p>åbningstid</p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Definition</td>
<td><blockquote>
<p>tidspunkter hvor kontaktpunktet kan anvendes</p>
</blockquote></td>
</tr>
<tr class="even">
<td>Anvendelsesnote</td>
<td>Fravær af angivelse af tidspunkter for kontakt betyder ikke at
kontaktpunktet ikke kan anvendes. Det indikerer enten at kontaktpunktet
kan anvendes på alle tidspunkter (eksempelvis e-mail) eller at der
aktuelt ikke er informationer om tidspunkter.</td>
</tr>
<tr class="odd">
<td>Domæne</td>
<td><blockquote>
<p>schema:ContactPoint</p>
</blockquote></td>
</tr>
<tr class="even">
<td>Udfaldsrum</td>
<td><blockquote>
<p>schema:OpeningHoursSpecification</p>
</blockquote></td>
</tr>
<tr class="odd">
<td>Multiplicitet</td>
<td><blockquote>
<p>0 - *</p>
</blockquote></td>
</tr>
</tbody>
</table>

### Specifikation af åbningstider (klasse)

##### *Vokabularets definition og beskrivelser*

| URI         | <http://schema.org/OpeningHoursSpecification>                                                                                                                                                                                                                                                                                                |
| ----------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Term        | Specifikation af åbningstider                                                                                                                                                                                                                                                                                                                |
| Kommentar   | En struktureret værdi, der giver information om åbningstiderne for et sted eller en bestemt tjeneste inde på et sted. Stedet er åbent, hvis egenskaben 'opens' er angivet og lukket ellers. Hvis værdien for egenskaben 'closes' er mindre end værdien for 'opens' egenskaben, så antages timeintervallet at strække sig over den næste dag. |
| Underklasse | schema:StructuredValue                                                                                                                                                                                                                                                                                                                       |

##### *Profilens restriktioner og beskrivelser* {#profilens-restriktioner-og-beskrivelser-50}

| Foretrukken term | Specifikation af åbningstider                                                  |
| ---------------- | ------------------------------------------------------------------------------ |
| Definition       | information om åbningstider som en del af beskrivelsen for en kontaktoplysning |

#### åbner

##### *Vokabularets definition og beskrivelser*

| URI        | <http://schema.org/opens>                                                      |
| ---------- | ------------------------------------------------------------------------------ |
| Term       | åbner                                                                          |
| Definition | det tidspunkt lokationen eller tjenesten åbner på den eller de angivne ugedage |
| Domæne     | schema:OpeningHoursSpecification                                               |
| Udfaldsrum | schema:Time                                                                    |

##### *Profilens restriktioner og beskrivelser* {#profilens-restriktioner-og-beskrivelser-51}

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th><blockquote>
<p>åbner</p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Domæne</td>
<td>schema:OpeningHoursSpecification</td>
</tr>
<tr class="even">
<td>Udfaldsrum</td>
<td>schema:Time</td>
</tr>
<tr class="odd">
<td>Multiplicitet</td>
<td>1 - 1</td>
</tr>
</tbody>
</table>

#### lukker

##### *Vokabularets definition og beskrivelser*

| URI        | <http://schema.org/closes>                                             |
| ---------- | ---------------------------------------------------------------------- |
| Term       | lukker                                                                 |
| Kommentar  | Stedets eller tjenestens lukketid på den eller de givne dag(e) i ugen. |
| Domæne     | schema:OpeningHoursSpecification                                       |
| Udfaldsrum | schema:Time                                                            |

##### *Profilens restriktioner og beskrivelser* {#profilens-restriktioner-og-beskrivelser-52}

| Foretrukken term | lukker                                                                            |
| ---------------- | --------------------------------------------------------------------------------- |
| Definition       | Stedets eller tjenestens lukketid på den eller de givne dag(e) i ugen.            |
| Anvendelsesnote  | Lukketid for den kontakt der repræsenteres i den kvalificerede kontaktinformation |
| Domæne           | schema:OpeningHoursSpecification                                                  |
| Udfaldsrum       | xsd:time                                                                          |
| Multiplicitet    | 1 - 1                                                                             |

#### gælder fra

##### *Vokabularets definition og beskrivelser*

| URI        | <http://schema.org/validFrom>                                                                                                                                                                                                |
| ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Term       | gælder fra                                                                                                                                                                                                                   |
| Kommentar  | Den dato, hvor værdien bliver gyldig.                                                                                                                                                                                        |
| Domæne     | schema:Permit eller schema:Certification eller schema:MonetaryAmount eller schema:Offer eller schema:OpeningHoursSpecification eller schema:LocationFeatureSpecification eller schema:Demand eller schema:PriceSpecification |
| Udfaldsrum | schema:DateTime eller schema:Date                                                                                                                                                                                            |

##### *Profilens restriktioner og beskrivelser* {#profilens-restriktioner-og-beskrivelser-53}

| Foretrukken term | gælder fra                                                         |
| ---------------- | ------------------------------------------------------------------ |
| Definition       | Den dato, hvor værdien bliver gyldig                               |
| Anvendelsenote   | Den dato, hvor den kvalificerede kontaktinformation bliver gyldig. |
| Domæne           | schema:OpeningHoursSpecification                                   |
| Udfaldsrum       | xsd:dateTime                                                       |
| Multiplicitet    | 0 - 1                                                              |

#### gælder indtil

##### *Vokabularets definition og beskrivelser*

| URI        | <http://schema.org/validThrough>                                                                                                                                                                      |
| ---------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Term       | gælder indtil                                                                                                                                                                                         |
| Domæne     | schema:PriceSpecification eller schema:MonetaryAmount eller schema:JobPosting eller schema:Offer eller schema:OpeningHoursSpecification eller schema:LocationFeatureSpecification eller schema:Demand |
| Udfaldsrum | schema:DateTime eller schema:Date                                                                                                                                                                     |

##### *Profilens restriktioner og beskrivelser* {#profilens-restriktioner-og-beskrivelser-54}

<table>
<colgroup>
<col style="width: 21%" />
<col style="width: 78%" />
</colgroup>
<thead>
<tr class="header">
<th>Foretrukken term</th>
<th><blockquote>
<p>gælder indtil</p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Definition</td>
<td>Dato, efter hvilken, værdien ikke længere er gyldig.</td>
</tr>
<tr class="even">
<td>anvendelsesnote</td>
<td>Den dato, hvor den kvalificerede kontaktinformation bliver
ugyldig.</td>
</tr>
<tr class="odd">
<td>Domæne</td>
<td>schema:OpeningHoursSpecification</td>
</tr>
<tr class="even">
<td>Udfaldsrum</td>
<td>xsd:dateTime</td>
</tr>
<tr class="odd">
<td>Multiplicitet</td>
<td>0 - 1</td>
</tr>
</tbody>
</table>

#### ugedag

##### *Vokabularets definition og beskrivelser*

| URI        | <http://schema.org/dayOfWeek>                                                |
| ---------- | ---------------------------------------------------------------------------- |
| Term       | ugedag                                                                       |
| Kommentar  | Den ugedag, som disse åbningstider er gældende for.                          |
| Domæne     | schema:OpeningHoursSpecification eller schema:EducationalOccupationalProgram |
| Udfaldsrum | schema:DayOfWeek eller schema:Text eller schema:URL eller schema:Role        |

##### *Profilens restriktioner og beskrivelser* {#profilens-restriktioner-og-beskrivelser-55}

| Foretrukken term | ugedag                               |
| ---------------- | ------------------------------------ |
| Definition       | den ugedag åbningstiderne gælder for |
| Domæne           | schema:OpeningHoursSpecification     |
| Udfaldsrum       | schema:DayOfWeek                     |
| Multiplicitet    | 1 - 1                                |

### Ugedag (klasse)

![](media/image34.emf){width="3.2368285214348207in"
height="1.2956528871391075in"}

Schema.orgs klasse schema:DayOfWeek er en klasse af enumerationer.
Schema.org har beriget klassen med de syv ugedage samt en pladsholder
for offentlige helligdage. Til brug for basisprofilen har der været
behov for at udvide med et antal dage og periodeangivelser som
illustreret nedenfor. Hele udvidelsen kan ses i 'Bilag H -- Typer af
dage'.

![](media/image35.emf)

##### *Vokabularets definition og beskrivelser*

| URI         | <http://schema.org/DayOfWeek>                                                                                                                                                                                                                                                                                                                          |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Term        | Ugedag                                                                                                                                                                                                                                                                                                                                                 |
| Kommentar   | Ugedagen, bruges eksempelvis til at angive, hvilken dag åbningstiderne for en OpeningHoursSpecification refererer til. Oprindeligt blev URLer fra 'GoodRelations' brugt (til 'Monday', 'Tuesday', 'Wednesday', 'Thursday' 'Friday', 'Saturday', 'Sunday' plus en særlig post til 'PublicHolidays'; disse er nu blevet integreret direkte i schema.org. |
| Underklasse | schema:Enumeration                                                                                                                                                                                                                                                                                                                                     |

#### betegnelse

##### *Vokabularets definition og beskrivelser*

| URI        | http://www.w3.org/2000/01/rdf-schema#label |
| ---------- | ------------------------------------------ |
| Term       | betegnelse                                 |
| Kommentar  | et menneskelæsbart navn for noget          |
| Domæne     | rdfs:Resource                              |
| Udfaldsrum | rdfs:Literal                               |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-56}

| Foretrukken term | betegnelse                                                                                                       |
| ---------------- | ---------------------------------------------------------------------------------------------------------------- |
| Definition       | et menneskelæsbart navn for noget                                                                                |
| Kommentar        | Af schema.org er ugedagene navngivet på engelsk. Den navngivning suppleres med en tilsvarende dansk navngivning. |
| Anvendelsesnote  | Bruges til at angive ugedagens navn.                                                                             |
| Domæne           | schema:dayOfWeek                                                                                                 |
| Udfaldsrum       | rdf:langString                                                                                                   |
| Multiplicitet    | 1 - \*                                                                                                           |

#### kommentar

##### *Vokabularets definition og beskrivelser*

| URI        | http://www.w3.org/2000/01/rdf-schema#comment |
| ---------- | -------------------------------------------- |
| Term       | kommentar                                    |
| Kommentar  | En beskrivelse af emneressourcen.            |
| Domæne     | rdfs:Resource                                |
| Udfaldsrum | rdfs:Literal                                 |

##### Profilens restriktioner og beskrivelser  {#profilens-restriktioner-og-beskrivelser-57}

| Foretrukken term | kommentar                         |
| ---------------- | --------------------------------- |
| Definition       | En beskrivelse af emneressourcen. |
| Domæne           | schema:dayOfWeek                  |
| Udfaldsrum       | rdf:langString                    |
| Multiplicitet    | 0 - \*                            |

## Eksempel på kontaktinformation

![](media/image36.emf)

##### JSON-LD-kode (uden context)

{

{

\"@id\" : \"xorg:unit-864\",

\"@type\" : \"org:OrganizationalUnit\",

\"contactPoint\" : \"xorg:contact-686\",

}

{

\"@id\" : \"xorg:contact-686\",

\"@type\" : \"schema:ContactPoint\",

\"identifier\" : \"Wegners Plads 2, 6270, Tønder\",

\"type\" : \"ci:FullAddress\",

\"contactType\" : {

\"@language\" : \"da\",

\"@value\" : \"Vi kan hjælpe dig med pas, kørekort, digitale
selvbetjeningsløsninger og meget mere.\"

},

\"hoursAvailable\" : \[ \"xorg:hours-890\", \"xorg:hours-319\",
\"xorg:hours-236\" \],

\"comment\" : {

\"@language\" : \"da\",

\"@value\" : \"Ekspedition af kørekort og pas er kun mulig i
Borgerservice i Tønder.\"

},

\"prefLabel\" : \"contact-686\"

}

{

\"@id\" : \"xorg:hours-319\",

\"@type\" : \"schema:OpeningHoursSpecification\",

\"closes\" : \"15:00:00\",

\"dayOfWeek\" : \[ \"schema:Monday\", \"schema:Tuesday\",
\"schema:Wednesday\" \],

\"opens\" : \"10:00:00\",

\"label\" : \"hours-319\",

\"prefLabel\" : \"hours-319\"

}

{

\"@id\" : \"xorg:hours-236\",

\"@type\" : \"schema:OpeningHoursSpecification\",

\"closes\" : \"18:00:00\",

\"dayOfWeek\" : \"schema:Thursday\",

\"opens\" : \"10:00:00\",

\"label\" : \"hours-236\"

}

{

\"@id\" : \"xorg:hours-890\",

\"@type\" : \"schema:OpeningHoursSpecification\",

\"closes\" : \"13:00:00\",

\"dayOfWeek\" : \"schema:Friday\",

\"opens\" : \"10:00:00\",

\"label\" : \"hours-890\",

\"prefLabel\" : \"hours-890\"

}

}

[^1]: <https://joinup.ec.europa.eu/collection/semic-support-centre>

[^2]: <https://semiceu.github.io/ADMS/releases/2.00/#Identifier>

[^3]: <https://semiceu.github.io/Core-Person-Vocabulary/releases/2.1.0/>

[^4]: <https://semiceu.github.io/Core-Business-Vocabulary/releases/2.00/>
