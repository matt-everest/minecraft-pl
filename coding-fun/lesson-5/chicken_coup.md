### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Kurnik

## Step 1
Agent musi położyć **2** warstwy po **9** bloków **żelaznych krat**. **4** boki muszą mieć **żelazne kraty**. Nie zapomnij użyć ``||agent:agent przesuń w górę||``, aby zbudować drugi poziom.

#### ~ tutorialhint
Na końcu będziesz mieć **3** polecenia ``||loops:powtórz||`` zagnieżdżone jedno w drugim. Upewnij się, że Agent ma w ekwipunku więcej niż 64 bloki!

```ghost
player.onChat("chicken", function () {
    for (let index = 0; index < 2; index++) {
        agent.setItem(IRON_BARS, 1, 1)
        for (let index = 0; index < 4; index++) {
            for (let index = 0; index < 9; index++) {
                agent.place(DOWN)
                agent.move(FORWARD, 1)
            }
            agent.turn(RIGHT_TURN)
        }
        agent.move(UP, 1)
    }
})

``` 
