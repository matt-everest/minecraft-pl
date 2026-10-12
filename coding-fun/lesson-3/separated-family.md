### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Rozdzielona rodzina!

## Step 1
Zaprogramuj Agenta, aby zbudował most nad szczeliną w lodzie. Upewnij się, że Agent ma w ekwipunku **64** bloki **desek dębowych**. 

#### ~ tutorialhint 
Nie zapomnij użyć **nie** w pętli **dopóki**. Zastanów się, gdzie Agent ma kłaść bloki. 


```ghost
player.onChat("family", function () {
    agent.setItem(PLANKS_OAK, 64, 1)
    agent.move(FORWARD, 1)
    while (!(agent.detect(AgentDetection.Block, FORWARD))) {
        agent.place(DOWN)
        agent.move(FORWARD, 1)
        agent.turn(LEFT_TURN)
    }
})

``` 
