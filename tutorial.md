# Special Minds Micro:Bit - Level 1

## Step 1

Vi skal starte med at lave en elektronisk terning. Til den skal vi bruge 3 blokke:

1. Én der registrerer når du ryster din terning (Micro:Bit).
2. Én der vælger et tilfældigt tal mellem 1 og 6.
3. Én der viser det valgte tal på displayet.

Tag Først en ``||input.onGesture||`` block der registrerer rystelser. 
```blocks
input.onGesture(Gesture.Shake, function () {
    
})
```

## Step 2

Herefter skal du bruge en block der kan vise et tal. Her skal du bruge en  ``||basic.showNumber||`` block.
```blocks
input.onGesture(Gesture.Shake, function () {
    basic.showNumber()
})
```
    

## Step 3

Til sidst skal programmet have at vide, at det skal vælge et tilfældigt tal mellem 1 og 6. Det gøres med en ``||math.pickRandom||`` block  

Efter at du har indsat blokken skal du huske at indstille den, så den vælger tal mellem 1 og 6
```blocks
input.onGesture(Gesture.Shake, function () {
    basic.showNumber(randint(1, 6))
})
```

## Step 4

Nu mangler du bare at at downloade programmet til din Micro:Bit


* for PXT/microbit
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
