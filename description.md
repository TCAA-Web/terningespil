# Lav et terningespil

### Besrkrivelse

Du skal kode et termingespil i JavaScript for to spillere. Der er en række regler til spillet som skal være opfyldt for at opgaven er løst.

### Reglerne:

To spillere skiftes til at slå med to terninger og den som slår det højeste antal øjne vinder runden.
Spillet spilles i tre runder. Hvis en runde ender uafgjort skal den slåes om.

- Scenarie 1:

```
Spiller 1 kaster med terningerne og slår 8
Spiller 2 kaster med terningerne og slår 5
Spiller 1 vinder runden og tildeles et point.
```

- Scenarie 2:

```
Spiller 1 kaster med terningerne og slår 12
Spiller 2 kaster med terningerne og slår 12
Runden ender uafgjort og ingen point tildeles.
```

### UI elementer

Terningerne skal vises på skærmen og der skal være en knap til at slå med terningerne.
Derudover skal der optræde en knap til at genstarte spillet.

Der skal være nogle få key UI elementer som score for player 1 og player 2, samt den aktuelle runde.
Der skal også være mulighed for at se de tidligere slag for henholdsvis player 1 og player 2.

### Hints:

- For at holde styr på hvilken spillers tur det er; kan man bruge en boolean `isPlayerOne=false`

- For at holde styr på hvilke terninger spillerne har slået kan du bruge et array. Arrays kan holde en række værdier i den rigtige rækkefølge. eks: `let playerOne = [5,4,8,6] `
  Her kan du nu både tjekke det sidste tal, hvor mange gange spilleren har slået (hvis tur det er), hvilken runde spilerne er nået til, samt vise de tidligere slag.

- Forsøg at skriv dine funktioner til spillet så genbrugelige som muligt. Hvis du eks. laver en funktion der tjekker om den ene spiller har slået højere end den anden, kan du med fordel lave nogle argumenter til funktionen der gør den genbrugelig til både spiller 1 og 2. Eks. `function hasPlayerWon(currentDice, previousDice) // returns true or false` istedet for `hasPlayerOneWon(), hasPlayerTwoWon()`
