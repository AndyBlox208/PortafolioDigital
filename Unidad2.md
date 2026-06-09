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
