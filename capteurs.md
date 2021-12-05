# Affichage de la valeur d'un capteur
La carte micro:bit possède un capteur de température
et un capteur de lumière intégrés.

## 1- Affichage capteur température

1.Dans le bloc Toujours, faire glisser un bloc 
montrer nombre.

2.Prendre dans le menu Entrée, un bloc "température (°C),
le glisser à la place du chiffre 0 dans montrer nombre.

La température doit s'afficher sur le panneau de LEDs !

```blocks
basic.forever(function () {
    basic.showNumber(input.temperature())
})
```


## 2- Affichage capteur lumière

Prendre cette fois dans le menu Entrée, un bloc
"niveau d'intensité lumineuse" et le mettre à la place
de température (en enlevant celui-ci).

```blocks
basic.forever(function () {
    basic.showNumber(input.lightLevel())
})
```


## 3- Affichage d'un capteurs avec condition

Modifier le programme précédent pour afficher la température
lorsque que l'on appuie sur le bouton A.

```blocks
input.onButtonPressed(Button.A, function () {
	
})
```

## 4- Affichage alterné température et lumière

Reprendre le dernier exercice et rajouter :


1.On doit afficher la température et à la suite un C (pour
Celsius), pause de 1s.

2.Puis montrer le niveau d'intensité lumineuse et afficher
lux à la suite.

TELECHARGER LE PROGRAMME POUR UN ESSAI ULTERIEUR
SUR LA CARTE.

```blocks
input.onButtonPressed(Button.A, function () {
    basic.showNumber(0)
    basic.showString("C")
    basic.pause(1000)
    basic.showNumber(0)
    basic.showString("lux")
})
```

