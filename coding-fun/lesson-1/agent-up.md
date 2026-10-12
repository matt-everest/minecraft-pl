### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @flyoutOnly 1
### @explicitHints 1


# Zaprogramuj Agenta, aby podszedł do złotej płytki!

## Step 1
Użyj poleceń ``||player:przy poleceniu czatu||`` i ``||agent:agent przesuń||``, aby zaprogramować Agenta w stronę złotej płytki. Możesz zaprogramować Agenta, aby poruszał się **w górę**. Gdy skończysz, naciśnij przycisk **Odtwórz**, aby skompilować kod. Przejdź do Minecrafta, aby uruchomić kod w grze.



```ghost
player.onChat("up", function () {
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
})

```  
