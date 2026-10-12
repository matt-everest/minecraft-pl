### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Oczyść roślinność!

## Step 1
Agent musi zniszczyć **8** bloków roślinności, idąc **do przodu**. Jest **16** rzędów roślinności do zniszczenia. Agent musi **8** razy ``||agent:zniszczyć blok z przodu||`` i ``||agent:przesunąć się do przodu||``. 
#### ~ tutorialhint 
```blocks
player.onChat("foliage", function () {
    for (let index = 0; index < 8; index++) {
        for (let index = 0; index < 8; index++) {
        	
        }
    }
})

```

```ghost
player.onChat("foliage", function () {
    for (let index = 0; index < 8; index++) {
        agent.destroy(FORWARD)
        agent.move(FORWARD, 1)
        for (let index = 0; index < 2; index++) {
            agent.move(FORWARD, 1)
            agent.turn(RIGHT_TURN)
        }
    }
})
``` 
