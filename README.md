# Om Region Hallands design guidelines
Detta repository innehåller koden för Region Hallands Design guildelines.

## Bidra gärna!
Vill du bidra till att bygga upp den här sajten? Hurra för det! Följ installationsguiden nedan för att få igång en lokal version av sajten och skicka sedan in en [pull request](https://help.github.com/articles/creating-a-pull-request/) när du är klar med dina förbättringar.

## Installation
Ta först hem reposet lokalt, gör sedan följande din terminalen:

### Installera Fractal
Fractal är det ramverk som vår dokumentation bygger på.

1. `npm install --save @frctl/fractal`
2. `npm i -g @frctl/fractal`

De två stegen ovan installerar Fractal och dess CLI verktyg

### Kör lokalt

2. `npm install`
2. `fractal start --synk`
3. Besök den URL som terminalen ger dig, troligtvis http://localhost:3000

### Bygg en dist

För att exportera ut Fractal till statiska filer som vi kan köra upp på http://design.regionhalland.se så behöver vi bygga en dist. Detta göra du genom att skriva `fractal build`när du står i `/`. Det i sin tur kommer att generera statiska HTML filer till `/build`som vi sedan kan lägga på vår server.

## Hur kan jag redigera innehåll på sajten?
Fractal applicerar [GitHub flavoured markdown](https://guides.github.com/features/mastering-markdown/) för allt innehåll.

### Redigera dokumentation m.m.
Allt innehåll, förutom komponenter, finns i `/docs/*` och mer detaljerad info om hur man redigerar dokument finns på [Fractals hemsida](https://fractal.build/guide/documentation/#a-simple-page)

### Redigera komponenter m.m.
[Redigering av komponenter](https://fractal.build/guide/components/) särskiljer sig något från övrig dokumentation så läs mer på Fractals egna sajt.

 ### Hantering av bilder m.m.
 Om du vill använda bilder m.m. i din dokumentation så lägg alla assets i `/assets/*` och hänvisa sedan till dem i din dokumentation t.ex. så här: `<img src="/assets/images/minbild.jpg" />`.
