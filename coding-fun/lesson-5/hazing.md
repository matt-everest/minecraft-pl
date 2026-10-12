### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Zabezpieczenie przed wilkami 

## Step 1
Agent musi ustawić **linkę potykacza**, aby wilki nie weszły do środka. Ustaw blok ``||agent:agent ustaw blok||`` na **linkę potykacza** i ustaw liczbę na **64**. Użyj bloku ``||loops:dopóki||`` i wstaw do niego warunek.  

#### ~ tutorialhint
Pamiętaj, aby użyć **nie** w swoim warunku. 

```blocks
player.onChat("hazing", function () {
    agent.setItem(TRIPWIRE, 64, 1)
    while (!(agent.detect(AgentDetection.Block, FORWARD))) {
    	
    }
})

``` 
```ghost
player.onChat("hazing", function () {
    agent.setItem(TRIPWIRE, 64, 1)
    while (!(agent.detect(AgentDetection.Block, FORWARD))) {
        agent.place(DOWN)
        agent.move(FORWARD, 1)
    }
})
```
