# Muros
![alt text](https://raw.githubusercontent.com/developerfab/netlogo/master/muros/muros_interface.png)

## WHAT IS IT?

Esta aplicacion es un ejemplo para hacer un pequeños análisis de comportamiento caotico al tener una población de 100 personas las cuales deben salir de un cuarto con una puerta de diferentes tamaños. Se hace uso de restricciones de movimiento y cambio de dirección en choques.

## HOW IT WORKS

###### limite-1 
Es el limite del mapa, ninguna tortuga puede sobrepasar los limites de color negro y en una zona amarilla muere.

###### setup
Crea las tortugas en el mundo seleccionador. Es llamada en cualquiera de las funciones mundo-1 o mundo-2.

###### crear-azar
Crea las tortugas en una posición al azar en -15 < x < -2 y -15 > y > 15.

###### crear-en-punto
Crea las tortugas en la posición x = -10 y = 0.

###### mundo-general
Crea los bordes del mundo,y las paredes internas. Es llamado por las funciones mundo-1 y mundo-2

###### mundo-1
Crea una puerta pequeña del tamaño de un patche en el mundo para que pasen las tortugas.

###### mundo-2
Crea una puerta pequeña del tamaño de 4 patches en el mundo para que pasen las tortugas.

###### caminar
Es la función que evalua 2 condiciones, la primera, si hay una tortuga frente a la que llama la función se llama la función girar, de lo contrario se llama la función paso.

###### paso
La tortuga da un paso en la dirreción en que mira y llama la función limite-1.

###### girar
La tortuga gira hacia la derecha un maximo de 180º y llama la función limite-1.

## HOW TO USE IT

###### Seleccionador de posición de inicio

Este seleccionador posee la variable global 'crear', con la cual se elige si se desean crear tortugas con posicion al azar o en una posición especifica. 

###### Mundos

El mundo 1 instancia el mundo-general y crea una puerta pequeña. Llama a la función mundo-1.

El mundo 2 instancia el mundo-general y crea una puerta de 4 patches de espacio. Llama a la función mundo-2.

###### Inicio

El boton iniciar permite ejecutar la simulación de forma continua.

###### Grafico pocisión vs tiempo

Este es un grafico que se pinta durante la ejecución de la simulación, compara el tamaño de la población a lo largo del tiempo.

## THINGS TO NOTICE

1. Compare los tiempos de salida de las tortugas entre los diferentes mundos.


## THINGS TO TRY
-

## EXTENDING THE MODEL

1. Cree un mundo con 2 o tres salidas y compare las respuestas.

## NETLOGO FEATURES

(interesting or unusual features of NetLogo that the model uses, particularly in the Code tab; or where workarounds were needed for missing features)

## RELATED MODELS

(models in the NetLogo Models Library and elsewhere which are of related interest)

## CREDITS AND REFERENCES

[ Funcion ramdom entre 2 valores] (http://netlogo-users.18673.x6.nabble.com/random-choice-general-question-td4863342.html)

[ Variables globales en netlogo ] (http://netlogo-users.18673.x6.nabble.com/How-can-I-define-a-value-into-a-global-variable-td4864733.html) 
autor: @developerfab
