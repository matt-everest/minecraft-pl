### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Znajdź młode!

## Step 1
Zaprogramuj Agenta, aby wykopał ścieżkę, nie wiedząc, jak jest długa, używając poleceń ``||loops:dopóki||`` i ``||agent:agent wykryj||``. Agent musi ``||agent:zniszczyć blok z przodu i u góry||``, abyś mógł przejść przez cały śnieg! Gdy skończysz, naciśnij przycisk **Odtwórz**, aby skompilować kod. Nie zapomnij uruchomić kodu w Minecrafcie. 

#### ~ tutorialhint 
Zwróć uwagę na kształty bloków kodu, gdy je ze sobą łączysz. Użyj ``||agent:agent przesuń do przodu||``.

```template
player.onChat("cub", function () {
    while (agent.detect(AgentDetection.Block, FORWARD)) {
    	
    }
})
```

```ghost
player.onChat("cub", function () {
    while (agent.detect(AgentDetection.Block, FORWARD)) {
        agent.destroy(FORWARD)
        agent.move(FORWARD, 1)
        agent.destroy(UP)
    }
})

``` 
