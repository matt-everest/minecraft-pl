### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @flyoutOnly 1
### @explicitHints 1


# Zaprogramuj Agenta, aby podszedł do złotej płytki!

## Step 1
Zaprogramuj Agenta, aby dotarł do złotej płytki. Ty musisz stać na swojej złotej płytce, a Agent musi stanąć na drugiej. Gdy skończysz, naciśnij przycisk **Odtwórz**, aby skompilować kod. Przejdź do Minecrafta, aby uruchomić kod.


```ghost
player.onChat("last", function () {
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
})
```  
