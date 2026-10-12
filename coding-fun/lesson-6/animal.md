### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true
### @explicitHints 1


# Aktywność zespołowa

## Step 1
Wybierz bloki potrzebne do zbudowania odpowiedniego domu dla zwierząt. Znajdziesz tu wszystkie bloki, których używaliśmy podczas lekcji!


```ghost
player.onChat("run", function () {
    agent.teleportToPlayer()
    agent.turn(LEFT_TURN)
    agent.move(FORWARD, 1)
    while (!(agent.detect(AgentDetection.Block, FORWARD))) {
    	
    }
    agent.place(FORWARD)
    agent.destroy(FORWARD)
    agent.setItem(GRASS, 1, 1)
    for (let index = 0; index < 4; index++) {
    	
    }
})

``` 
