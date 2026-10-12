### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Bambusowa granica

## Step 1
Przygotowaliśmy dla Ciebie kod startowy.  Najpierw spróbuj go uruchomić. Ostatecznym celem jest posadzenie bambusa wzdłuż **4** boków działki pandy. 

```template
player.onChat("bamboo", function () {
    agent.setItem(BAMBOO, 64, 1)
    for (let index = 0; index < 16; index++) {
        agent.place(DOWN)
        agent.move(FORWARD, 1)
    }
    agent.turn(LEFT_TURN)
})
```
