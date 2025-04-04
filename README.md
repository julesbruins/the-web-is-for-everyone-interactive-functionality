# Interactive Functionality

Ontwerp en maak voor een opdrachtgever een interactieve toepassing die voor iedereen toegankelijk is

De instructie vind je in: [INSTRUCTIONS.md](https://github.com/fdnd-task/the-web-is-for-everyone-interactive-functionality/blob/main/docs/INSTRUCTIONS.md)


## Inhoudsopgave

  * [Beschrijving](#beschrijving)
  * [Gebruik](#gebruik)
  * [Kenmerken](#kenmerken)
  * [Ontwerpkeuzes](#ontwerpkeuzes)
  * [Installatie](#installatie)
  * [Bronnen](#bronnen)
  * [Licentie](#licentie)

## Beschrijving
Wat al stond was een website met 4 verschillende rouwtaken, waarvan elke overzichtspagina met rouwtaak zijn eigen thema en afbeeldingen droeg. Bij elke rouwtaak zijn de bijbehorende verschillende opdrachten te vinden. Deze kun je ook allemaal openen door op de 'start oefening' button te klikken. Dan kom je op een detailpagina van de opdracht terecht. Afgelopen weken hebben we gewerkt aan het toevoegen van een post. Dit geeft de mogelijkheid zelf een community drop te plaatsen en deze terug te zien, omdat deze opgeslagen wordt in de database. Dit is ook weer een detailpagina van de exercisepagina.
<!-- Bij Beschrijving staat kort beschreven wat voor project het is en wat je hebt gemaakt -->
<!-- Voeg een mooie poster visual of video toe 📸 -->
<!-- Voeg een link toe naar GitHub Pages 🌐-->
[De live website om zelf te bekijken!](https://the-web-is-for-everyone-interactive-mmsf.onrender.com)


https://github.com/user-attachments/assets/ad06fb28-dd7e-4153-9f13-e3d1be7b02ef




## Gebruik
<!-- Bij Gebruik staat de user story, hoe het werkt en wat je er mee kan. -->
Als gebruiker van drop en heal wil ik ervaringen met de opdrachten van anderen kunnen lezen en zelf een ervaring delen zodat je weet dat je niet alleen bent.
Je klikt op de link naar community drop, hier kan je eerst de community drops lezen die al gedeeld (gepost) zijn. Vervolgens klik je op 'plaats bericht' waar je doorgelinkt wordt naar een pagina waar je je eigen ervaring kan schrijven en achterlaten. Je wordt dan weer terug gestuurd naar de community drops. 

## Kenmerken
<!-- Bij Kenmerken staat welke technieken zijn gebruikt en hoe. Wat is de HTML structuur? Wat zijn de belangrijkste dingen in CSS? Wat is er met JS gedaan en hoe? Misschien heb je iets met NodeJS gedaan, of heb je een framework of library gebruikt? -->

- Allereerst wordt er een post in liquid verwerkt in een formulier. 
- Vervolgens wordt er doormiddel van de server een post aangemaakt. Deze is makkelijk terug te vinden in de [code met uitleg](https://github.com/julesbruins/the-web-is-for-everyone-interactive-functionality/blob/fd992460dd555769918defafb9f77021d40fb51b/server.js#L86-L105). De server verwerkt deze post en stuurt deze naar de database.
- Dit kun je dan weer uitwerken in liquid waardoor de post uit de database ook daadwerkelijk zichtbaar wordt.

- Verder wordt er in de [server](https://github.com/julesbruins/the-web-is-for-everyone-interactive-functionality/blob/fd992460dd555769918defafb9f77021d40fb51b/server.js#L65) nog gekeken hoeveel berichten er zijn, en dit kan dan weer in de [liquid](https://github.com/julesbruins/the-web-is-for-everyone-interactive-functionality/blob/fd992460dd555769918defafb9f77021d40fb51b/views/exercise.liquid#L12) dynamisch aangegeven worden. Zo wordt er dynamisch aangegeven hoeveel community drops er zijn.
- Ook is er nog gebruik gemaakt van een succes state in [Javascript](https://github.com/julesbruins/the-web-is-for-everyone-interactive-functionality/blob/fd992460dd555769918defafb9f77021d40fb51b/public/scripteen.js#L1-L12). Deze geeft een melding met een bevestiging dat er een nieuwe post is gemaakt doormiddel van de [server](https://github.com/julesbruins/the-web-is-for-everyone-interactive-functionality/blob/fd992460dd555769918defafb9f77021d40fb51b/server.js#L100) weer.
- Tot slot heb ik een [empty state](https://github.com/julesbruins/the-web-is-for-everyone-interactive-functionality/blob/18b8243b8bcf82bca4d4ffce4346ca705012dff9/views/community-drops.liquid#L31-L33) toegevoegd. Deze geeft een melding wanneer er ergens nog geen community drops geplaatst. Zo weet je dat de pagina correct geladen is maar er gewoon nog geen drops zijn bij die opdracht.
<img width="383" alt="Screenshot 2025-04-04 at 15 30 35" src="https://github.com/user-attachments/assets/f01c41d4-94db-40e6-9409-ae6f34e9293f" />


## Ontwerpkeuzes
Ik heb een responsive ontwerp gemaakt met meerdere breakpoints. Ook heb ik [container queries](https://github.com/julesbruins/the-web-is-for-everyone-interactive-functionality/blob/18b8243b8bcf82bca4d4ffce4346ca705012dff9/public/styles/task.css#L129-L140) toegepast op de overzichtspagina's van de taken. Dit zorgt ervoor dat wanneer het scherm nog te klein is om meerdere opdrachten naast elkaar te zetten, dat ze wel een andere styling krijgen. De styling veranderd aan de hand van de breedte van het object in plaats van de breedte van het scherm.



https://github.com/user-attachments/assets/5eb7dccb-1058-4647-ba18-9c4b06b36857




## Installatie
<!-- Bij Installatie staat hoe een andere developer aan jouw repo kan werken -->
In dit project wordt gebruik gemaakt van NodeJS. Om aan dit project te werken moet NodeJS geïnstalleerd zijn. Eenmaal geïnstalleerd kan het project geopend worden in de code editor.

Voer in de terminal `npm install` uit om alle afhankelijkheden te installeren.

Voer vervolgens `npm start` uit om de server te starten.

Ga in je browser naar http://localhost:8000 om het project te bekijken.

## Bronnen

## Licentie

This project is licensed under the terms of the [MIT license](./LICENSE).
