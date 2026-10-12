### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Wielka szczelina!

## Step 1
Zaprogramuj Agenta, aby **zbudował most** nad szczeliną w lodzie. Użyj bloku ``||agent:agent ustaw blok lub przedmiot||``, aby upewnić się, że Agent ma w ekwipunku potrzebne materiały. Wybierz **dąb** jako materiał budowlany i **64** jako **liczbę bloków**. ``||loops:dopóki||`` Agent **nie** wykrywa bloków w dole, zaprogramuj go tak, aby kładł deski dębowe **w dół** i przesuwał się **do przodu**, tworząc most.    


```template
player.onChat("chasm", function () {
    agent.setItem(PLANKS_OAK, 1, 1)
    agent.move(FORWARD, 1)
    while (!(agent.detect(AgentDetection.Block, DOWN))) {
    	
    }
})
```

```ghost
player.onChat("chasm", function () {
    agent.setItem(PLANKS_OAK, 64, 1)
    agent.move(FORWARD, 1)
    while (!(agent.detect(AgentDetection.Block, FORWARD))) {
        agent.place(DOWN)
        agent.move(FORWARD, 1)
    }
})

``` 

