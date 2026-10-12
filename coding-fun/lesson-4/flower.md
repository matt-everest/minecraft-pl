### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true
### @explicitHints 1


# Upiększ teren!

## Step 1
Musisz posadzić **14 mleczy** wzdłuż **4** boków kryjówki. Agent może posadzić **14** mleczy z jednej strony. 

#### ~ tutorialhint 
Nie zapomnij wybrać liczby w poleceniu ``||agent:agent ustaw blok||``. 


```ghost
player.onChat("flower", function () {
    for (let index = 0; index < 4; index++) {
        for (let index = 0; index < 14; index++) {
            agent.setItem(YELLOW_FLOWER, 64, 1)
            agent.place(DOWN)
            agent.move(FORWARD, 1)
        }
        agent.turn(RIGHT_TURN)
    }
})

``` 
