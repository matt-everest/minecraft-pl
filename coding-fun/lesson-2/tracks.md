### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @flyoutOnly 1
### @explicitHints 1


# Zaprogramuj Agenta, aby szedł wzdłuż żółwich śladów!

## Step 1
Przesuń Agenta wzdłuż żółwich śladów do bramek, używając bloku ``||agent: agent przesuń do przodu||``. Gdy skończysz, naciśnij przycisk **Odtwórz**, aby skompilować kod. Nie zapomnij uruchomić kodu w Minecrafcie. 

```ghost
player.onChat("tracks", function () {
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
})
for (let index = 0; index < 4; index++) {
    	
 }
``` 
