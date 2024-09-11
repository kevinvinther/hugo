---
title: 'En kort introduktion til Anki'
date: 2024-09-11T11:14:12+02:00
draft: false
ShowToc: true
TocOpen: true
params:
  ShowBreadCrumbs: true
---

**Mål**: Denne artikel vil give en kort introduktion til huskekortsprogrammet Anki. Introduktionen vil bestå af følgende:

* Motivation for hvorfor Anki kan være et gavnligt program
* Hvornår man skal bruge Anki
* Oversigt over brugeroverfladen
* Add-ons og delte decks

Anki kan downloades på følgende links:
* Windows/Mac/Linux: https://apps.ankiweb.net/
* iOS: https://apps.apple.com/us/app/ankimobile-flashcards/id373493387
* Android: https://play.google.com/store/apps/details?id=com.ichi2.anki&hl=en

# Introduktion

Anki er et huskekortsprogram der kan bruges til at huske alt der kan nedskrives på et huskekort. Ankis algoritme tillader dig at huske uden at du behøver gøre andet, end at bruge programmet hver dag, og kigge de kort igennem, som programmet vil have dig til at kigge igennem. Dette gør det til et fantastisk program til at bruge til studie, selvstudie, arbejde m.m. Du kan for eksempel bruge det til at lære et nyt sprog, huske alle verdens lande, huske beviser og meget mere.

# Hvorfor Anki?

Anki er et huskekortsprogram ligesom *quizlet*, *remnote*,[^1] *memrise*, og *supermemo*, samt mange flere. Hvad der primært adskiller *Anki* fra mange af disse er at den:
1. Er *open source*. Det vil sige at koden er frit tilgængelig.
2. Bruger *spaced repetition*. 
3. Har en simpel, letforståelig brugeroverflade.

Der er naturligvis flere ting end disse, men disse er nogle af de mest primære til hvorfor man skulle vælge *Anki* fremfor konkurrenterne.

## Huskekort

Der er flere forskellige typer af huskekort du kan bruge i Anki, men i denne gennemgang vil vi kun kigge på 2: *Basic* og *Cloze*:

Et *basic* kort er blot et kort bestående af en forside og en bagside. Forsiden kan for eksempel være "Hvad er hovedstaden af Tyskland?" hvortil bagsiden vil være svaret: "Berlin".

Et *cloze* kort lyder mere kompliceret i teorien, men er også utroligt nemt at forstå. Her har du ikke mere end én side, men på den side kan du *blokere* ord eller sekvenser af ord (samt tekst, tal, etc). Vi kommer til at kigge dybere på hvordan dette fungerer senere. Et eksempel kan være følgende sætning: "Mitokondriet er cellens energiproducerende organel, hvor det primært genererer ATP gennem cellulær respiration." Denne kan laves om til et huskekort hvor **fed skrift** indikerer tekst vi blokerer. "**Mitokondriet** er cellens **energiproducerende organel**, hvor det primært genererer **ATP** gennem **cellulær respiration**."

Denne vil resultere i 4 huskekort, et hvor man ikke kan se ordet "Mitokondriet", et hvor man ikke kan se "Energiproducerende Organel" etc. Det vil derfor se ud således, når du gennemgår kortet som ønsker Mitokondriet som svar:

> [...] er cellens energiproducerende organel, hvor det primært genererer ATP gennem cellulær respiration.

Her er dit mål så at huske hvad der skal stå bag de tre punktummer.

## Spaced Repetition

Det primære salgsargument for Anki er dens *spaced repetition*[^2] algoritme. En spaced repetition-algoritme optimerer huskeevne af huskekort. Det vil altså sige, at hvis du laver 100 kort til Anki, alle omkring et emne du gerne vil huske i lang tid, så kan algoritmen planlægge hvornår du skal kigge på dem igen, på en sådan måde hvor du vil kunne huske dem igen næste gang du ser dem. 

Premisset med en sådan algoritme, er at vi glemmer information afhængigt af hvor ofte vi ser informationen. Hvis du har set dit huskekort en enkelt gang, vil du glemme den hurtigt. Hvorimod, hvis du ser dent10 gange med et passende (variabelt) mellemrum mellem disse gange, vil du kunne huske det bedre.

{{< image "En kort introduktion til Anki - Spaced Repetition.png" >}}

(Billede fra https://www.osmosis.org/learn/Spaced_repetition)

Dette virker, fordi du gennemgår en proces der kaldes *active recall*,[^3] hvor du aktivt forsøger at huske noget, fremfor at genlæse det igen, og igen. Dette forsøg på at huske, styrker din evne til at finde præcis den information frem igen, når du skal til at bruge det. Anki's algoritme forsøger at give dig dit huskekort *lige inden du glemmer det*. Derfor kræver det ekstra meget energi, men du husker det også bedre, fordi du styrker evnen til at finde præcis den information frem hver gang. 

Derudover tager Anki's algoritme hvor godt du kan huske kortet med i betragtning. Det er ikke bare "Det kunne jeg ikke huske", eller "Det kunne jeg godt huske". Afhængigt af hvor godt du husker det (*Slet ikke*, *Hårdt*, *Okay*, *Nemt*), justerer den på nogle variabler bag scenen, der siger både hvornår du skal se kortet igen, men også hvad der skal ske næste gang. For eksempel, hvis jeg husker et kort dårligt, så får jeg det måske igen i morgen. På dette tidspunkt, har Anki allerede udregnet hvad der så vil ske, hvis jeg husker kortet dårligt igen, og giver mig kortere tid før jeg ser kortet igen.

## Brugervenlighed

Anki er utroligt nemt at bruge. Vi har ikke kigget på brugeroverfladen endnu, men du behøver ikke at trykke på mere end et par tastaturknapper for at lave og gennemgå kort. 

Brugeroverfladen er simpel, og let at forstå. Der er ikke en masse unødvendige funktioner, som du aldrig kommer til at bruge. Du kan dog, hvis det lyster, tilføje sådanne funktioner ved brug af *add-ons*, som vi kommer ind på senere.

# Hvornår Skal Man Bruge Anki?

Anki er kun godt **hvis du skal huske noget**. Hvis dit mål med anki er at lære noget nyt, kan du ikke bruge det til noget. Du skal allerede havde lært informationen, og forstået den, før du kan forsøge at huske den. Hvis du sætter en svær ligning ind, og ikke forstår den endnu, vil du aldrig kunne huske den. 

Hvis jeg lige har læst en overfladisk gennemgang af anden verdenskrig, ville følgende kort være passeligt at tilføje:

> **Forside**
> Hvornår sluttede 2. verdenskrig?
> **Bagside**
> 2. September 1945

Hvorimod, hvis du gennemgår præsentationen til en forelæsning du ikke har været til, hvor følgende står:

>  $T$ er transformations matrixen til skalering.

Men du hverken ved hvad skalering eller en transformations matrix er, så får du ikke noget ud af kortet. Du vil ikke kunne huske det, fordi du ikke forstår de ord. Du vil altid kunne forsøge at lave et kort, men det vil kræve markant mere af dig, at forsøge at huske det.

# Hvordan Bruger Man Anki?

{{< image "En kort introduktion til Anki - Brugeroverflade.png" >}}


Når du starter Anki på computer for første gang, vil du finde en brugeroverflade meget lignende den på billedet over. Egentlig burde den eneste forskel være, at du kun har ét "deck", hvor der udfra står "0 0 0".

## Decks

**1 - Decks**
Her finder du skærmen du er på lige nu. Der er her dine "decks" er. Decks er blot samlinger af huskekort, kategoriseret på en sådan måde, at de blive sammenlignet i samme "session". Det vil altså sige, at hvis du laver et deck der hedder "Lineær Algebra", og lægger kort ind med information om både lineær algebra og hunderacer, vil du både få huskekort om lineær algebra og hunderacer, når du gennemgår kortene. 

Der er flere fordele ved at organisere dine kort på en sådan måde, fremfor at have ét monolitisk deck, hvori du har alle dine kort. En af de vigtigste er, at du kan ændre på indstillingerne for hvert deck, og se statistikker for hvert deck. Vi vil dog ikke gå ind på indstillinger i denne guide. 

## Tilføj Nye Kort

**2 - Add**
Her kan du tilføje nye huskekort til dine decks. 
{{< image "En kort introduktion til Anki - Add.png" >}}


Her kan du skrive hvad der skal være på hhv. forsiden og bagsiden af dit huskekort. På den øverste bjælke ser du "Type" og "Deck". Her bestemmer du hvilken type kort (e.g. Basic eller Cloze) du har lyst til at lave, og under hvilket deck de skal tilhøre. For eksempel kan man se på skærmprintet at jeg er ved at lave et simpelt huskekort under typen "Basic" til mit deck omhandlende *Geometric Computation*. Dette er et underdeck, hvilket vi ikke vil gå i detaljer med her, blot vid at du kan lave dem ved at trække dine decks ind i hinanden på "Decks" skærmen. 

På næstnederste bjælke ser du teksten "Tags". Herunder kan du lave forskellige tags, til at kategorisere dine huskekort endnu mere. Hvis du skriver huskekort til en forelæsning, kan du foreksempel lave tagget "Forelæsning9-9" for at sige at det er forelæsningen fra den 9. September. Du kan også lave undertags ved at bruge "::". For eksempel kan du lave tagget "ComputationalGeometry::Forelæsning9-9". Ved denne er Forelæsning9-9 et "undertag" af ComputationalGeometry.

På den nederste bjælke til højre kan du se knapperne "Add", "History" og "Close". Vi kigger kun på Add og Close. Add tilføjer kortet til decket, og close lukker vinduet du kigger på. I stedet for at klikke på Add hver gang du har lavet et nyt kort, kan du også blot trykke Ctrl + Enter. Derudover kan du skifte hvilken "input" du skriver i ved at trykke tab. Så du kan starte i "Front" og skrive dit input, e.g. "Hvor mange stater har USA?" trykke tab, og skrive "50", efterfulgt af Ctrl + Enter. Så har du tilføjet et kort. 

### Brug Af Cloze

{{< image "En kort introduktion til Anki - Cloze.png" >}}


Det ovenstående skræmprint viser et "Cloze" kort, hvori der står: "Amerika har {{c1::50}} stater". Når du gennemgår dette kårt vil du se "Amerika har [...] stater." på forsiden og "Amerika har 50 stater." på bagsiden. Du kan også lave mere end én blokering ved at lave flere instanser af {{c1::abc}}, eller du kan lave flere kort (som beskrevet tidligere) ved at forøge *x* i {{cx::abc}}, e.g. {{c2::kort2}}, {{c3::kort3}}. Du kan også blande disse sammen, så du har flere af samme *cx* og flere hvor *x* er anderledes, såsom følgende: 

"**{{c1::Napoléon Bonaparte}}** (født **{{c2::15. august 1769}}**, død **{{c3::5. maj 1821}}**) var Frankrigs førstekonsul fra 1799 og var franskmændenes kejser under navnet **{{c1::Napoléon I}}** fra den 18. maj 1804 – 11. april 1814 og igen 20. marts – 22. juni 1815. Han erobrede og regerede det meste af det vestlige og centrale Europa."[^4]

Når du gennemgår kort 1 vil du se følgende: 
"**[...]** (født 15. august 1769, død 5. maj 1821) var Frankrigs førstekonsul fra 1799 og var franskmændenes kejser under navnet **[...]** fra den 18. maj 1804 – 11. april 1814 og igen 20. marts – 22. juni 1815. Han erobrede og regerede det meste af det vestlige og centrale Europa."

Kort 2 og 3 vil give lignende resultater, men med de andre blokerede tekste. Når du laver et *cloze*-huskekort kan du bruge Ctrl + Shift + C for at lave en ny blokering, og Ctrl + Alt + Shift + C, for ikke at forøge tallet. 

## Database Af Huskekort

**3 - Browse**
På denne tab vil du have en oversigt over alle de huskekort du har lavet. Her kan du også ændre og slette huskekort, samt andre egenskaber. Disse vil vi dog ikke komme ind på.

## Statistik

**4 - Stats**
Herinde vil du kunne se statistik for dine forskellige decks, eller for alle decks tilsammen. Du kan vælge et specifikt deck øverst. Hvis du shift-trykker på "Stats" vil du få den gamle version, hvilket nogle *add-ons* bruger til at vise statistik relevant for dem.

## Synkronisering

**5 - Sync**
Anki har en gratis, indbygget funktionalitet til at kunne synkronisere dine huskekort. Det eneste det kræver er at du opretter en bruger. Dermed vil du også kunne tage dine huskekort til din mobil, eller en anden computer. Når du har lavet en bruger, skal du blot trykke "sync" for at Anki synkroniserer dine kort.

## Dine Decks

**6 - Dine Decks**
Her kan du se dine decks. Jeg har forklaret det meste om dem i første sektion af dette. Dog kan du se til højre tre kolonner: *New*, *Learn* og *Due*. New er nye huskekort du endnu ikke har set. *Learn* er huskekort du ikke har lært ordentligt endnu. Disse kan også være kort du har lært, men har glemt og derfor skal se dem igen i dag. *Due* er kort du skal se i dag, som du har lært tidligere.

Det er også her du gennemgår dine huskekort. Ved at trykke på en af dine decks, kommer du til en skærm lignende denne (antagelse på at du har lavet mindst ét huskekort til decket): 


{{< image "En kort introduktion til Anki - Study Now.png" >}}


Her skal du trykke "Study Now" for at begynde din session. 

{{< image "En kort introduktion til Anki - Huskekort.png" >}}


Dit kort kommer ikke til at se sådan her ud, men det kommer til at ligne i strukturen. Denne guide vil ikke gennemgå "styling", hvilket er hvad der gør at kortet kan se anderledes ud. 

Nederst på kortet kan du se "Show Answer". Du skal først trykke på dette når du har forsøgt at finde svaret til dit kort. Når du har gjort det, får du disse 4 valgmuligheder: 
{{< image "En kort introduktion til Anki - Valgmuligheder.png" >}}


Alt efter hvor godt du har husket skal du vælge en af disse. Jeg har en svag huskeregel, der afgører hvordan jeg vælger disse:
* **Again**: Hvis jeg slet ikke kunne huske kortet, eller huskede forkert
* **Hard**: Hvis det tog mig mere end 15 sekunder, og jeg måske var i tvivl om det var A eller B, men kom til den rette konklusion
* **Good**: Hvis det tog mig mere end 5 sekunder (men jeg huskede det indenfor 15 sekunder), og jeg huskede det korrekt.
* **Easy**: Hvis jeg huskede korrekt indenfor 5 sekunder.

Ud fra hvordan du vælger, kan du se at der går kortere eller længere tid. Ved dette specifikke kort, ville jeg se kortet igen om 10 minutter hvis jeg slet ikke kunne huske det. Jeg ville derimod først se det om 2.1 måneder hvis jeg huskede det godt. Her er notationen *m* = minutter, *d* = dage, *mo* = måneder, *y* = år.

## Lav Et Nyt Deck

**7 - Create Deck**
Her laver du et nyt deck. For denne guide er alt du behøver at finde et navn til det.

# Add-ons Og Delte Decks

## Add-ons

Add-ons er funktionaliteter til Anki lavet udenfor Anki's grund. Du kan se de forskellige Add-ons, ved i øverste bjælke (Med File, Edit, View, etc.) at trykke følgende: **Tools -> Add-ons -> Get Add-ons -> Browse Add-ons**. dette vil føre dig til siden https://ankiweb.net/shared/addons. Find et addon, og find dens kode, og tryk denne kode ind i feltet i det vindue du fandt "Browse Add-ons" knappen på:

{{< image "En kort introduktion til Anki - Installer Addon.png" >}}


Når du trykker "OK" installerer anki add-onen, og ved genstart er den integreret i Anki.

Der er ingen add-ons der er nødvendige for Anki, og jeg vil derfor anbefale at kigge igennem de forskellige add-ons på siden, og se om der er nogen der kan hjælpe dig specifikt. Der er stor sandsynlighed for, at når du har brugt anki i noget tid, vil der være nogle ting du ikke synes er specielt fede, eller du mangler. Ved at kigge add-ons igennem, kan du med høj sandsynlighed finde en der hjælper på dit problem.

## Delte Decks

Der ligger mange decks online, som folk allerede har lavet og delt. Du kan oftest finde dem på https://ankiweb.net/shared/decks. Du kan importere dem til Anki ved at downloade dem, og dobbelt-trykke på den fil du downloader, og derefter bliver den importeret til Anki.

Jeg vil dog ikke anbefale at bruge denne metode til noget udover almen viden såsom geografi. Når du laver dine egne kort husker du dem bedre, og du ved at de fungerer for dig, og at du ved præcis hvad der står deri. Hvis du downloader et andet deck kan vedkommende have lavet kortene på en uforståelig måde, eller du har ikke viden nok til at forstå kortene.

# Viderelæsning

Ved lyst til mere læsning, kan  [den officielle dokumentation](https://docs.ankiweb.net/) bruges.

[^1]: Selve programmet er ikke et huskekortsprogram, men har en funktion til integration af huskekort.
[^2]: Dansk: Gentagelse med mellemrum
[^3]: Dansk: Aktiv genkaldelse
[^4]: Taget fra Wikipedia 11-9-24. **Fed Skrift** er blot for fremhævelse.
