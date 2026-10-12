### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration false 
### @explicitHints 1


# Wyżej!

## Step 1
Zaprogramuj Agenta, aby zbudował wieżę z bloków **dębowych** o wysokości **10** bloków. Najpierw upewnij się, że Agent ma **64** bloki **desek dębowych**, używając polecenia ``||agent:agent ustaw blok lub przedmiot||``. Zaprogramuj Agenta, aby kładł deski dębowe **do przodu**, **w lewo** i **w prawo**, używając bloku ``||agent:agent umieść||``. Po położeniu bloków Agent musi **przesunąć się w górę**.  

#### ~ tutorialhint 
Spróbuj użyć bloku ``||loops:powtórz||`` i zmień liczbę na **10**. 

## Step 2
Zaprogramuj Agenta, aby zszedł **w dół** z wieży i zbudował **drabinę** o wysokości **10** bloków. Drabina jest potrzebna, żebyś Ty mógł wspiąć się na górę!

#### ~ tutorialhint 
Nie zapomnij wybrać **64** bloków **drabiny** w ekwipunku Agenta za pomocą bloku ``||agent: agent ustaw blok||``, aby Agent mógł ją postawić. 


```ghost
player.onChat("tower", function () {
    agent.move(FORWARD, 1)
    agent.setItem(LADDER, 64, 1)
    for (let index = 0; index < 10; index++) {
        agent.place(FORWARD)
        agent.move(UP, 1)
    }
    agent.move(DOWN, 10)
})

``` 


