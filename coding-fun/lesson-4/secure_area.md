### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Zabezpiecz teren

## Step 1
Zaprogramuj Agenta, aby zbudował **dębowy płot**. Agent musi kłaść bloki **dębowego płotu** po prawej stronie, niszczyć przeszkody i iść do przodu. Płot powinien mieć **17 bloków** długości. 

#### ~ tutorialhint
Upewnij się, że Agent kładzie bloki po prawej stronie i niszczy bloki po lewej. 

```blocks
player.onChat("fence", function () {
    agent.setItem(OAK_FENCE, 64, 1)
    for (let index = 0; index < 17; index++) {
            }
})
```
```ghost
player.onChat("fence", function () {
    agent.setItem(OAK_FENCE, 64, 1)
    for (let index = 0; index < 17; index++) {
        agent.place(RIGHT)
        agent.destroy(FORWARD)
        agent.move(FORWARD, 1)
    }
})
``` 

