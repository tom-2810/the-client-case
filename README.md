> _Fork_ deze leertaak en ga aan de slag. Onderstaande outline ga je gedurende deze taak in jouw eigen GitHub omgeving uitwerken. De instructie vind je, zoals altijd, in: [docs/INSTRUCTIONS.md](docs/INSTRUCTIONS.md)

# Titel
<!-- Geef je project een titel en schrijf in één zin wat het is -->

## Inhoudsopgave

  * [Beschrijving](#beschrijving)
  * [Kenmerken](#kenmerken)
  * [Bronnen](#bronnen)
  * [Licentie](#licentie)

## Beschrijving

### 🥇 WCAG richtlijnen
Met deze tool kan een organisatie concrete informatie vinden over toegankelijkheids richtlijnen.
Daarnaast helpt het de organisatie om beter te begrijpen waarom en hoe die richtlijnen hun website/app helpt om toegankelijker te worden.
Deze richtlijnen zijn afkomstig van het WCAG die vanaf 2025 wettelijk verplicht gesteld worden.

Om de richtlijnen in de zien, kiest u een principe door er naartoe te scrollen of te selecteren in de navigatie. Vervolgens klikt u op een richtlijn, zoals "Richtlijn 1.1 Tekstalternatieven". Dan komt de bijbehorende korte uitleg tevoorschijn met daaronder het "waarom en hoe".

### 🖥️ Desktop
De tool bestaat uit één pagina, waardoor de informatie overzichtelijk blijft.
Met een simpele navigatie aan de zijkant is snel bladeren mogelijk.
![image](https://user-images.githubusercontent.com/112861614/195764590-20e2700c-198a-434d-b92f-96fbc28c1a97.png)

### 📱 Smartphone
Ook kan de tool op andere apparaten gebruikt worden, zoals een smartphone en tablet.
De layout blijft vrijwel gelijk, maar de navigatie is naar beneden verplaatst. Dit maakt meer ruimte vrij voor de principes, zodat deze leesbaar blijven.
Daarnaast is deze manier van navigeren vergelijkbaar met een app, waardoor het bekend is bij de gebruiker.
![image](https://user-images.githubusercontent.com/112861614/195765112-d8ee55c6-cb09-4db7-91bf-d95d08cdad40.png)

### 🙋 User flow
Hier volgen nog wat user flow afbeeldingen.

Selecteer een principe bij "Snel naar: ".
![image](https://user-images.githubusercontent.com/112861614/195765641-8e7b774d-f768-45c5-ac15-5bca51ba8bec.png)

Selecteer een richtlijn.
![image](https://user-images.githubusercontent.com/112861614/195765724-e435afdd-f2f9-4774-a703-bdfd1009b593.png)

### 🌐 Link naar Toolgankelijk
https://tom-2810.github.io/the-client-case/

## Kenmerken
<!-- Bij Kenmerken staat welke technieken zijn gebruikt en hoe. Wat is de HTML structuur? Wat zijn de belangrijkste dingen in CSS? Wat is er met Javascript gedaan en hoe? Misschien heb je een framwork of library gebruikt? -->
### Grid

Door middel van `display: grid;` is het `main` element opgesteld. Op de dekstop versie staat de content links en de `#side-nav` rechts. Deze verhouding is `grid-template-columns: 2fr 1fr;`. Daarnaast zal de content niet groter worden dan `max-width: 55rem;` om de regels compact te houden. De `#side-nav` zal niet groter worden dan `max-width: 30rem;`. Diezelfde `#side-nav` heeft `position: sticky;` en `top: 5rem` hierdoor scrollt het element eerst een stuk naarboven, totdat het de `#top-nav` binnen de `header` nadert. Dan blijft de `#side-nav` op dezelfde positie op het scherm, waardoor deze altijd bereikbaar blijft.

De `#side-nav` maakt gebruikt van bijvoorbeeld `<a href="#waarneembaar">`, om naar Principe 1: Waarneembaar te navigeren.

De richtlijnen worden getoont als `details` met daarin een `summary` die het kopje een titel geeft. Zodra hierop word geklikt klapt deze open en verschijnt de bijbehorende informatie.

Zodra het scherm kleiner word dan `max-width: 1060px` zal de `#side-nav` verdwijnen en komt er een `bottom-nav` voor in de plaats. Deze is `position: fixed;` en blijft dus altijd onderaan in beeld.


## Bronnen

## Licentie

![GNU GPL V3](https://www.gnu.org/graphics/gplv3-127x51.png)

This work is licensed under [GNU GPLv3](./LICENSE).
