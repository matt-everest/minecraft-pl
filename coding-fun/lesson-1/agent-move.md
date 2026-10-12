### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @flyoutOnly 1
### @explicitHints 1


# Zaprogramuj Agenta, aby przeszedł do złotej płytki!

## Step 1
Wybierz polecenie ``||player:przy poleceniu czatu||`` i zmień jego nazwę z **run** na **1**. Wybierz blok ``||agent: agent przesuń do przodu||`` i przeciągnij go do wnętrza polecenia ``||player:przy poleceniu czatu||``. Zmień **liczbę** kroków Agenta na **3**, aby Agent dotarł do złotej płytki. Gdy skończysz, naciśnij przycisk **Odtwórz**, aby skompilować kod, potem przejdź do Minecrafta, naciśnij **t** i wpisz **1**.

#### ~ tutorialhint 
Możesz zmienić liczbę kroków Agenta, zmieniając liczbę w bloku ``||agent: agent przesuń||``. Możesz też użyć bloku ``||agent: agent obróć się||``, aby obrócić Agenta w lewo lub w prawo.



```ghost
player.onChat("1", function () {
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
})

``` 
