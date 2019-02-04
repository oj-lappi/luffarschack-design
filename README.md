# Luffarschack på webben

## Mål 

 - En webbapplikation med enkelt gränssnitt
 - Minimalistiskt design-språk: symboler, färger och animationer över text och instruktioner
 - Bra känsla när man använder applikationen

 

## Skärmar: överblick

 - En landing-page var man får konfigurera hurdant spel man vill spela
   - konfigurationselement i en lista: en rad - en konfiguration
   - fortsätt-knapp
 - Spelbrädan
   - motståndar-avatar i övre höger hörn: robot eller mänska
   - spelar-avatar i nedre vänster hörn
   - en spelbräda 
   - ifall spelaren väntar på motståndaren, en länk som kan delas

  
## Funktionella krav
 
### Konfigurationsskärmen

 Spelaren får själv välja en spelkonfiguration med dessa variabler:

  - vilken symbol spelaren använder ( X börjar alltid ) 
    - X
    - O
    - ingen skillnad
  - motståndare:
    - robot
    - människa
  - om människa, hur välja motståndare:
   - match-making
   - dela länk (länk-symbolen)
  - spelplanens storlek (endast kvadrater):
    - 3x3
    - 4x4
    - 5x5
    - 10x10
  - _ALTERNATIV_ spelplanens storlek: välj sidlängd (input i `[]`, andra talet fylls i automatiskt): 
        `[5] x 5` 
        `[3] x 3`
  - hur många symboler i rad som behövs för att vinna ( input-box, med +/- knappar)
    - min 3
    - max sidlängd
 
  När spelaren konfigurerat spelet färdig, trycker spelaren på fortsätt-nappen

### Spelskärmen

 - Om spelaren valt att dela länk visas en länk spelaren kan dela länken med en annan spelare
 - Spelet spelas mot en svart bakgrund, så att fokus är på planen
 - När man väljer nästa position, lyser alla andra egna symboler upp som kan forma en rad med den symbolen
  - t.ex. en animation, eller en grann, positiv färg (deepskyblue)
 - När spelet tar slut:
  - lyser den vinnande raden upp i en animation
   - t.ex. en pulserande animation som ändrar storlek och färg av symbolerna i den vinnande raden
  - faller "konfetti" ner från toppen av skärmen
  - visas en knapp som låter spelaren gå tillbaka till konfigurationsskärmen
 
### Allmänt

 - En nightmode/daymode knapp, som byter från ljus till mörk bakgrund och vv.

## Projektet
 
Projektet kommer att vara en prototyp. Om möjligt försöker vi få så mycket av spelet implementerat som möjligt, men fokus är på designen. Vi gör åtminstone nägra skärmar.

### Projektmedlemmar

Oskar Lappi

Martin Asplund

Magnus Thölix

### Risker

Otydliga krav

Mycket grafiskt arbete
