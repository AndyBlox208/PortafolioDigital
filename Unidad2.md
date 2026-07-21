[<< Regresar](https://github.com/AndyBlox208/PortafolioDigital/blob/main/Encabezado.md)

[Unidad 3 >>](Unidad3.md)
# Unidad 2
## Estructuras condicionales
Las estructuras condicionales son el corazón de la lógica en la programación. Son las que permiten que un programa deje de ser una lista aburrida de instrucciones secuenciales y empiece a "tomar decisiones" basadas en si una condición es verdadera o falsa.

Básicamente, le dicen a la computadora: "Si pasa X, haz Y; pero si pasa Z, haz W".
### 1. Estructura Condicional Simple (Si - Entonces)
Es la forma más básica. Evalúa una condición: si se cumple (es verdadera), ejecuta un bloque de código. Si no se cumple (es falsa), simplemente se salta ese bloque y continúa con el resto del programa.
#### Pseudocódigo:
Si (condicion) Entonces<br>
&emsp;// Acción o acciones a realizar si la condición es verdadera<br>
FinSi<br>
#### Diagrama de flujo:
![Imagen alt](https://github.com/AndyBlox208/PortafolioDigital/blob/de3e33e10cad9df7c5d85c23174d9d95c3c1e458/foto031.jpg)
### 2. Estructura Condicional Doble (Si - Entonces - Sino)
Aquí ya le damos una alternativa al programa. Si la condición se cumple, se hace una cosa; si no se cumple (por descarte), se ejecuta un camino alternativo.
#### Pseudocódigo:
Si (condicion) Entonces<br>
&emsp;// Acciones si la condición es VERDADERA<br>
Sino<br>
&emsp;// Acciones si la condición es FALSA<br>
FinSi<br>
#### Diagrama de flujo:
![Imagen alt](https://github.com/AndyBlox208/PortafolioDigital/blob/e1974b2b5aff36a8a919d43d165f482372cb9a6a/foto033.jpg)
### 3. Estructura Condicional Anidada (Estructuras dentro de otras)
¿Qué pasa si tienes más de dos opciones? Puedes meter un Si - Entonces dentro de otro Si - Entonces. Esto te permite evaluar múltiples condiciones en cadena.
#### Pseudocódigo:
Si (condicion1) Entonces<br>
&emsp;// Acciones si condicion1 es verdadera<br>
Sino<br>
&emsp;Si (condicion2) Entonces<br>
&emsp;&emsp;// Acciones si condicion1 fue falsa, pero condicion2 es verdadera<br>
&emsp;Sino<br>
&emsp;&emsp;// Acciones si ambas condiciones fueron falsas<br>
&emsp;FinSi<br>
FinSi<br>
#### Diagrama de flujo:
![Imagen alt](https://github.com/AndyBlox208/PortafolioDigital/blob/625e3757df3fcd01527728e49f5e5cf82db7525f/foto035.jpg)
### 4. Estructura Condicional Múltiple (Según o En caso de)
Cuando tienes una sola variable que puede tomar muchos valores específicos (como un menú de opciones o los días de la semana), usar muchos Si anidados se vuelve una pesadilla visual. Para eso existe la estructura múltiple (el famoso Switch en lenguajes como C++ o Java).
#### Pseudocódigo:
Segun (variable) Hacer<br>
&emsp;valor1:<br>
&emsp;&emsp;// Acciones para valor1<br>
&emsp;valor2:<br>
&emsp;&emsp;// Acciones para valor2<br>
&emsp;De Otro Modo:<br>
&emsp;// Acciones si no coincide con ningún valor anterior<br>
FinSegun<br>
#### Diagrama de flujo:
![Imagen alt](https://github.com/AndyBlox208/PortafolioDigital/blob/9f49aaceb7501e557274f87246e8c4d28fd80882/1-diagra-de-flujo-estructura-selectiva-multiple-768x402.png)
## Estructuras repetitivas
Sirven para ejecutar un bloque de instrucciones una y otra vez mientras se cumpla una condición o hasta que se alcance un número determinado de repeticiones. Imagina tener que escribir Escribir "Hola Mundo" 500 veces... para eso existen los bucles.
### 1. Estructura Mientras (Bucle While)
Es una estructura pre-test, lo que significa que primero evalúa la condición y, si es verdadera, ejecuta el código de su interior. Si la condición es falsa desde el principio, el bloque de código nunca se ejecutará.
#### Pseudocódigo:
Mientras (condicion) Hacer<br>
&emsp;// Instrucciones que se repiten<br>
FinMientras<br>
#### Diagrama de flujo:
![Imagen alt](https://github.com/AndyBlox208/PortafolioDigital/blob/479b4ed70bb8deccdee86a84bfae7e354ffb1da8/foto042.jpg)
### 2. Estructura Repetir - Hasta Que (Bucle Do-While / Repeat-Until)
A diferencia del anterior, este es un bucle post-test. Esto significa que primero ejecuta las instrucciones y después evalúa la condición. Por lo tanto, el código de adentro se va a ejecutar al menos una vez, pase lo que pase.
#### Pseudocódigo:
Repetir<br>
&emsp;// Instrucciones que se ejecutan al menos una vez<br>
Hasta Que (condicion_de_parada)<br>
#### Diagrama de flujo:
![Imagen alt](https://github.com/AndyBlox208/PortafolioDigital/blob/3ec1c7af6612e56722e644c13bc9bc25beaa58ca/repetir-hasta-que-diagrama-de-flujo.png)
### 3. Estructura Para (Bucle For)
Esta estructura es la mejor opción cuando sabes de antemano exactamente cuántas veces quieres que se repita el código. Automáticamente maneja una variable contadora, su valor inicial, su valor final y cuánto aumenta en cada vuelta (paso).
#### Pseudocódigo:
Para variable_control <- valor_inicial Hasta valor_final Con Paso incremento Hacer<br>
&emsp;// Instrucciones que se repiten<br>
FinPara<br>
#### Diagrama de flujo:
![Imagen alt](https://github.com/AndyBlox208/PortafolioDigital/blob/ae03a0e10070ea838d449339ae01b0634db86b05/foto033%20(1).jpg)
## Ejercicio con estructura condicuonal
### Planteamiento de problema
Deseamos poder realizar un programa que nos permita ingresar cualquier numero positivo y entonces sacar el factorial de este numero y tambien mostrar como la cantidad va llegando poco a poco a la respuesta, el programador debe ingeniarselas para poder realizar este problema.
### Amalisis del problema
Analizando el porblema podemos identificar que necesitaremos 1 datos de entrada como el numero que va a ingresar el usuario, 1 contador que no va a ayudar a tener control del ciclo y 1 acumulador que nos va a ayudar a ir acumulando las multiplicaciones y haci poder sacar el resultado final.
### Diagrama de flujo
![Imagen alt](https://github.com/AndyBlox208/PortafolioDigital/blob/4953970e08c17e5d6200fb749fbaf781b85e2def/Captura%20de%20pantalla%202026-06-09%20205635.png)
### Codificacion
![Imagen alt](https://github.com/AndyBlox208/PortafolioDigital/blob/5508023344e2a574bf5a64cccd8a62c17c6fa147/Captura%20de%20pantalla%202026-06-09%20210156.png)
### Validacion
| n | a | acum  | Salida |
| :---: | :---: | :---: | :---: |
| 0 | 0 | 1 |  |
| 5 | 1 | 1 | 1 |
| 5 | 2 | 1 | 2 |
| 5 | 3 | 2 | 6 |
| 5 | 4 | 6 | 24 |
| 5 | 5 | 24 | 120 |
## Principales dificultades y reflexión crítica
Una de mis principales dificultades a la hora de realizar este codigo fue hacer la multiplicacion, pues los resultados eran certeros mas no el procedimiento, pues las multiplicaciones que se hacian progresivamente no eran correctas y eso se tenia que corregir.
Gracias a este tipo de trabajos me ayuda a darme cuenta la importancia de los ciclos repetitivos y las condiciones que nos permiten tener un mejor control de todo el programa y lo que queremos realizar, ademas de ahorrar memoria y hacer mas rapidos los programas. 
