# Special Minds Micro:Bit - Level 1

## Step 1

Først skal vi lige kigge på brugerfladen her:  
1. Du kan for det første se en virtuel udgave af en Micro:Bit. Den kan du bruge til at teste på. F.eks. vil der dukke en knap op der hedder Shake (Ryst) som simulerer at den bliver rystet.  
2. Du kan også se en menu med et blåt, et pink og et lilla menupunkt. De indeholder Basic blokke, input blokke og matematiske blokke.  
3. Ved siden af er der et "arbejdsbord" som du bruger til at lave på koden ved at trække dine blokke ind. Der er i forvejen to blå blokke som du ikke skal bruge endnu.  
4. Klik på knappen "Næste" helt ude i højre side, for at fortsætte denne tutorial.

## Step 2

Vi skal starte med at lave en elektronisk terning. Til den skal vi bruge 3 blokke:

1. Én der registrerer når du ryster din terning (Micro:Bit).
2. Én der vælger et tilfældigt tal mellem 1 og 6.
3. Én der viser det valgte tal på displayet.

Tag Først en ``||input.onGesture||`` block der registrerer rystelser. 
```blocks
input.onGesture(Gesture.Shake, function () {
    
})
```

## Step 3

Herefter skal du bruge en block der kan vise et tal. Her skal du bruge en  ``||basic.showNumber||`` block.
```blocks
input.onGesture(Gesture.Shake, function () {
    basic.showNumber()
})
```
    

## Step 4

Til sidst skal programmet have at vide, at det skal vælge et tilfældigt tal mellem 1 og 6. Det gøres med en ``||math.pickRandom||`` block  

Efter at du har indsat blokken skal du huske at indstille den, så den vælger tal mellem 1 og 6
```blocks
input.onGesture(Gesture.Shake, function () {
    basic.showNumber(randint(1, 6))
})
```

## Step 5

Nu mangler du bare at at downloade programmet til din Micro:Bit
