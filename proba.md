# Felvillanó ledek
Felvillanó led

## Első feladat
Összesen 25 led villantható fel. 
A koordináták a sorok és oszlopok számpárjával adhatók meg. Az A gomb lenyomására kapcsold fel a [0,0] koordinátában lévő ledet!  
![mc01](https://user-images.githubusercontent.com/40439488/127630823-d15a95d4-222e-4435-83ed-e26d66101e9d.png) 
```blocks
input.onButtonPressed(Button.A, function () {
    led.plot(0, 0)	
})
```

## Második feladat
Készítsd el az X és y változókat!
```blocks
let x = 0
let y = 0
input.onButtonPressed(Button.A, function () {
    x = 0
    y = 0
    led.plot(0, 0)
})
```

## Harmadik feladat
Állítsd be az x és y változók értékét 0-ra (ha jelenleg nem annyi), és módosítsd a felkapcsol blokkot: konkrét számok helyett a két változó kerüljön ide!
```blocks
let x = 0
let y = 0
input.onButtonPressed(Button.A, function () {
    x = 0
    y = 0
    led.plot(x, y)
})
```

## Negyedik feladat
Először az első sor 5 ledjét fogjuk egy ciklus segítségével felkapcsolni. 
Az oszlopok (x) értékét minden felvillanás után eggyel növelni kell.  
![mc02](https://user-images.githubusercontent.com/40439488/127650720-4a190641-667a-466c-ba75-d4f3a6b599b1.png)
```blocks
let x = 0
let y = 0
input.onButtonPressed(Button.A, function () {
    x = 0
    y = 0
    for (let index = 0; index < 5; index++) {
        led.plot(x, y)
        x += 1
    }
})
```