### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Bambusowa kryjówka

## Step 1
Zaprogramuj Agenta, aby posadził **3** bloki bambusa z każdej strony piaszczystego placu. Dodaj polecenie ``||agent: agent obróć się||``, aby Agent mógł ukończyć aktywność. 

#### ~ tutorialhint
Powinny być 2 pętle **powtórz**, jedna wewnątrz drugiej.
 
```ghost
player.onChat("bamboo", function () {
    for (let index = 0; index < 3; index++) {
        agent.setItem(BAMBOO, 64, 1)
        agent.place(DOWN)
        agent.move(FORWARD, 1)
    }
    agent.turn(RIGHT_TURN)
})
```


