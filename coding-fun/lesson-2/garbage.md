### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @flyoutOnly 1
### @explicitHints 1


# Zaprogramuj Agenta, aby zebrał wszystkie śmieci!

## Step 1
Użyj Agenta, aby oczyścić żółwie ślady, korzystając z bloków ``||agent: agent zniszcz||`` i ``||agent:agent zbierz wszystko||``. Spróbuj użyć bloku ``||loops:powtórz||``, aby kod był bardziej wydajny. Gdy skończysz, naciśnij przycisk **Odtwórz**, aby skompilować kod. Nie zapomnij uruchomić kodu w Minecrafcie. 


```ghost
player.onChat("garbage", function () {
    for (let index = 0; index < 4; index++) {
        agent.turn(LEFT_TURN)
        agent.move(FORWARD, 1)
        agent.destroy(FORWARD)
        agent.collectAll()
    }
})
```
