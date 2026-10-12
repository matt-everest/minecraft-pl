### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Bydło

## Step 1
Przyjrzyj się kodowi startowemu i spróbuj go uruchomić. Ten kod pozwala prowadzić Agenta bez liczenia bloków. Zobacz, którą drogą Agent musi pójść, i dokończ sekwencję kodu z prawidłowymi skrętami Agenta. Upewnij się, że Agent dotrze do **złotej płytki**.  

```template
player.onChat("sheep", function () {
    while (!(agent.detect(AgentDetection.Block, FORWARD))) {
        agent.move(FORWARD, 1)
    }
    agent.turn(LEFT_TURN)
})

``` 

