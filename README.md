# Squad Page 1i - Twitch - Team Fun
We hebben in sprint 7 als Team de opdracht gekregen om een Squad Page te gaan bouwen met behulp van NodeJS, Express, JSON en Liquid. In JSON worden [alle data](https://fdnd.directus.app/items/person/) getoont die uit de FDND Database komen.

Als team hebben wij gewerkt aan verschillende interacties zoals de: Zoekbalk, Sorteer en Filter knoppen waar je op squads kan sorteren en van oud naar jong of van jong naar oud kan filteren. En als laatst een comment sectie waar je een berichtje kan achterlaten bij elk student/docent (UGC - User Generated Content).

Bij het maken van een website is het belangrijk dat het responsive is voor alle apparaten (Mobiel, Tablet en Desktop) maar ook de toegankelijkheid voor alle gebruikers. Als team hebben wij ons best gedaan om deze belangrijke eigenschappen te toepassen aan onze website. En om deze eigenschappen te controleren maken we gebruik van een WCAG Audit en een Kleur Contrast test.

**Het team (Fun)**

In dit team werken 3 eerste jaars Frontend Design & Development studenten studenten.

- [Tin Nguyen](https://github.com/WebTins)

- [Semih Demir](https://github.com/Hexterty46)

- [Kate Jadi](https://github.com/Kitkatisvibing)

## Inhoudsopgave

## Beschrijving

[Website](https://connect-your-tribe-team-squad-page-kvl8.onrender.com/)

De squadpage is eerst ontworpen en daarna gebouwd met interacties. De hoofdpagina toont een lijst aan studenten met een foto, naam, bijnaam, geboortedatum en schoenmaat. En in de hoofdpagina is het mogelijk om te gaan sorteren op squads, filteren op leeftijd en naar de chatpagina te gaan.

<img width="1800" height="760" alt="all-devices-black" src="https://github.com/user-attachments/assets/888f24fc-eecf-4bfd-8490-ff07460dd247" />

> Mockup van gemaakte Squad Page - Index

<img width="1800" height="760" alt="all-devices-black (1)" src="https://github.com/user-attachments/assets/e2548cb1-fa33-4380-8484-fc440ad4fb4b" />

> Mockup van gemaakte Squad Page - Comment section

**Responsiveness**

Responsiveness van de website is belangrijk voor alle apparaten en daarom hebben wij ook eerst op mobiele versie gewerkt om onze responsivness uit te breiden op tablet en desktop. We hebben ervoor gezorgd dat de cards onder elkaar in 1 kolom staan op mobiel en voor tablet worden er 2 kolommen getoont. Voor desktop worden zo'n 3-4 kolommen aan cards weergegeven.

https://github.com/user-attachments/assets/de7b1136-7213-49ec-9c40-7cce5053f746

**Toegankelijkheid**

Als team hebben wij ons best gedaan om de website toegankelijk te maken door middel van kleuren te gebruiken die voldoen aan het contrast dat leesbaar is voor iedereen. Om de toegankelijk te kunnen testen hebben we een [WCAG Audit](https://github.com/WebTins/connect-your-tribe-team-squad-page/issues/15) gedaan met een Lighthouse test op Google Chrome. Ook hebben we een handmatige test uitgevoerd die we moeten voldoen van het A11Y Project.

### Filter op Squads

Het doel van de filter interactie is dat als je op "Squad 1i" of "Squad 1j" klikt, dat de cards worden gefiltered op de leden in de squad. Ook kan je weer terug sorteren naar "Alle squads.

De filter knoppen zijn gemaakt met [routes](https://github.com/WebTins/connect-your-tribe-team-squad-page/blob/722ffd12b304e7c8d8c2b4858d66e180b299167e/server.js#L131-L170) die in NodeJS staan.

#### <ins>Feedforward & Feedback</ins>
Feedforward filter Squads:
- Er staat een knop bovenaan de pagina in het paars
- Met een hover over de filter krijgt de knop een lichtere kleur

Feedback filter naam:
- Na het klikken op de filter Squad 1i/Squad 1j/Alle Squads, worden alle leden getoont die in de Squad zitten

https://github.com/user-attachments/assets/31025ed8-d315-49d6-9616-a3e67bc6749d

### Sorteer op leeftijd

Het doel van de sorteer interactie is dat als je op "Jong" of "Oud" klikt, dat de cards worden sorteerd op jong/oud leeftijd.

De sorteer knoppen zijn gemaakt met[routes](https://github.com/WebTins/connect-your-tribe-team-squad-page/blob/e4b85f74c3b56bce7b028e057cc16c9e95fe0876/server.js#L172-L219) die in NodeJS staan.

#### <ins>Feedforward & Feedback</ins>

Feedforward sorteer Jong/Oud:
- Er staat een knop bovenaan de pagina in het paars
- Met een hover over de sorteer knop krijgt de knop een lichtere kleur

Feedback filter items:
- Na het klikken op de sorteer knop worden leden getoont van jong naar oud of van oud naar jong.

https://github.com/user-attachments/assets/581fb10b-d19b-46ce-9650-957595967429


### Zoekbalk

Naast het sorteren en filteren is het ook mogelijk om een specifieke persoon te gaan zoeken in de zoekbalk. In de [home route](https://github.com/WebTins/connect-your-tribe-team-squad-page/blob/08a8215264fbf981fa328ffb1b115ffe409a2db7/server.js#L27-L29) die in server.js staat wordt een query search uitgevoerd die de naam filtert met de inhoud die je meegeeft.

https://github.com/user-attachments/assets/6eddaa6b-a69d-4634-b745-a59f4827b67c

### Twitch Chat

Onze theme voor de website is geïnspireerd door "Twitch" een online streamingplatform waar je kan livestreamen en chatten. Het doel van de twitch chat is dat je een bericht kan achterlaten bij elke persoon die je aanklikt op de homepagina. Je kan je eigen naam achterlaten met een berichtje wanneer je op de chat pagina bent beland.

https://github.com/user-attachments/assets/b007fb9e-04f8-41b9-8f37-e43eb8d88e4b

## Kenmerken

In dit project is er gebruik gemaakt van HTML, CSS, JS, NodeJS, Express, JSON en Liquid.

**Active**

De sorteer/filter buttons krijgen een "active state" wanneer je erop klikt. Dit zorgt voor duidelijkheid waar je nu bent op de pagina en wat je hebt aangelikt.

https://github.com/user-attachments/assets/443420e7-3b42-4f71-bebd-4afcdcd2b5ae

**Else placeholder**

Leden zonder een profielfoto in de database krijgen als vervanging een Patrick foto.

<img width="326" height="493" alt="image" src="https://github.com/user-attachments/assets/a5f846dc-8e09-4d0b-800f-c2e42b1c629c" />

## Code conventies

### Ademnruimte

In onze code maken wij gebruik van ademruimte dat ervoor zorgt dat het lezen van code leesbaar is en te volgen is. Na elke element wordt een witregel gemaakt om het element duidelijk scheidbaar te tonen. En elementen in een elementen worden met 1 tab uitgespreid om te laten zien dat het in het parent element hoort.

[Voorbeeld](https://github.com/WebTins/connect-your-tribe-team-squad-page/blob/ea308ee98aa5b659e00e4d0e0119d300e8557b63/views/index.liquid#L7-L30)

## Volgorde HTML en CSS nesting

Bij onze code conventies houden wij rekening met de vologorde van de HTML structuur die ook in het CSS bestand op volgorde wordt gehouden, hierdoor wordt het lezen van code volgbaar en leesbaar. In onze CSS nesten wij code die in het parent element/class horen. Dit zorgt voor een duidelijke structuur dat het lezen makkelijker maakt.

## Custom properties

Wij maken gebruik van custom-properties zodat we niet steeds code hoeven te herhalen (DRY). De custom properties krijgen een duidelijke naamgeving in kebabcase zoals `--light-accent`.

## Class naamgeving

De classes die wij aanmaken worden allemaal in het Engels geschreven met kebab-cases. Dit maakt het lezen makkelijker omdat je een scheiding maakt tussen woorden die niet leesbaar zijn aan elkaar.
