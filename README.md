# Interactive Functionality

Ontwerp en maak voor een opdrachtgever een interactieve toepassing die voor iedereen toegankelijk is

De instructie vind je in: [INSTRUCTIONS.md](https://github.com/fdnd-task/the-web-is-for-everyone-interactive-functionality/blob/main/docs/INSTRUCTIONS.md)


## Inhoudsopgave

  * [Beschrijving](#beschrijving)
  * [Gebruik](#gebruik)
  * [Kenmerken](#kenmerken)
  * [Installatie](#installatie)
  * [Bronnen](#bronnen)
  * [Licentie](#licentie)

## Beschrijving
Wat al stond was een website met 4 verschillende rouwtaken, waarvan elke overzichtspagina met rouwtaak zijn eigen thema en afbeeldingen droeg. Bij elke rouwtaak zijn de bijbehorende verschillende opdrachten te vinden. Deze kun je ook allemaal openen door op de 'start oefening' button te klikken. Dan kom je op een detailpagina van de opdracht terecht. Afgelopen weken hebben we gewerkt aan het toevoegen van een post. Dit geeft de mogelijkheid zelf een community drop te plaatsen en deze terug te zien, omdat deze opgeslagen wordt in de database. Dit is ook weer een detailpaagina van de exercisepagina.
<!-- Bij Beschrijving staat kort beschreven wat voor project het is en wat je hebt gemaakt -->
<!-- Voeg een mooie poster visual of video toe 📸 -->
<!-- Voeg een link toe naar GitHub Pages 🌐-->
[De live website om zelf te bekijken!](https://the-web-is-for-everyone-interactive-mmsf.onrender.com)

## Gebruik
<!-- Bij Gebruik staat de user story, hoe het werkt en wat je er mee kan. -->
Als gebruiker van drop en heal wil ik ervaringen met de opdrachten van anderen kunnen lezen en zelf een ervaring delen zodat je weet dat je niet alleen bent.
Je klikt op de link naar community drop, hier kan je eerst de community drops lezen die al gedeeld (gepost) zijn. Vervolgens klik je op 'plaats bericht' waar je doorgelinkt wordt naar een pagina waar je je eigen ervaring kan schrijven en achterlaten. Je wordt dan weer terug gestuurd naar de community drops. 

## Kenmerken
<!-- Bij Kenmerken staat welke technieken zijn gebruikt en hoe. Wat is de HTML structuur? Wat zijn de belangrijkste dingen in CSS? Wat is er met JS gedaan en hoe? Misschien heb je iets met NodeJS gedaan, of heb je een framework of library gebruikt? -->
Ik heb gebruik gemaakt van 
- Allereerst wordt er een post in liquid verwerkt in een formulier. 
- Vervolgens wordt er doormiddel van de server een post aangemaakt. Deze is makkelijk terug te vinden in de [code met uitleg](https://github.com/julesbruins/the-web-is-for-everyone-interactive-functionality/blob/fd992460dd555769918defafb9f77021d40fb51b/server.js#L86-L105). De server verwerkt deze post en stuurt deze naar de database.
- Dit kun je dan weer uitwerken in liquid waardoor de post uit de database ook daadwerkelijk zichtbaar wordt.

- Verder wordt er in de [server](https://github.com/julesbruins/the-web-is-for-everyone-interactive-functionality/blob/fd992460dd555769918defafb9f77021d40fb51b/server.js#L65) nog gekeken hoeveel berichten er zijn, en dit kan dan weer in de [liquid](https://github.com/julesbruins/the-web-is-for-everyone-interactive-functionality/blob/fd992460dd555769918defafb9f77021d40fb51b/views/exercise.liquid#L12) dynamisch aangegeven worden. Zo wordt er dynamisch aangegeven hoeveel community drops er zijn.
- Tot slot is er nog gebruik gemaakt van een succes state in [Javascript](https://github.com/julesbruins/the-web-is-for-everyone-interactive-functionality/blob/fd992460dd555769918defafb9f77021d40fb51b/public/scripteen.js#L1-L12). Deze geeft een melding met een bevestiging dat er een nieuwe post is gemaakt doormiddel van de [server](https://github.com/julesbruins/the-web-is-for-everyone-interactive-functionality/blob/fd992460dd555769918defafb9f77021d40fb51b/server.js#L100) weer. 

## Installatie
<!-- Bij Installatie staat hoe een andere developer aan jouw repo kan werken -->
In dit project wordt gebruik gemaakt van NodeJS. Om aan dit project te werken moet NodeJS geïnstalleerd zijn. Eenmaal geïnstalleerd kan het project geopend worden in de code editor.

Voer in de terminal `npm install` uit om alle afhankelijkheden te installeren.

Voer vervolgens `npm start` uit om de server te starten.

Ga in je browser naar http://localhost:8000 om het project te bekijken.

## Bronnen

## Licentie

This project is licensed under the terms of the [MIT license](./LICENSE).
