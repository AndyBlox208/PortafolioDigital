[<< Regresar](https://github.com/AndyBlox208/PortafolioDigital/blob/main/Encabezado.md)
# Unidad 3
## Modularidad
La modularidad es el principio de dividir un programa grande y complejo en fragmentos más pequeños, independientes y enfocados en una sola tarea. A estos fragmentos los llamamos módulos (también conocidos como funciones, métodos o procedimientos).

Diseñar el código de esta manera evita la repetición, facilita encontrar errores y permite que varios programadores trabajen en el mismo proyecto sin estorbarse.

Cuando el programa principal necesita usar un módulo, le envía información a través de parámetros. Existen dos formas de enviar esta información:
### 1. Pase de parámetro por valor
Cuando pasas un parámetro por valor, el programa le entrega a la función una copia exacta de la variable original. Si la función modifica ese dato, solo está alterando su copia local; la variable original permanece intacta.

**Ejemplo:**

<img width="567" height="395" alt="image" src="https://github.com/user-attachments/assets/98f9399b-936b-4fe7-bb24-b3efa2e20208" />

### 2. Pase de parámetro por referencia
Cuando pasas un parámetro por referencia, no envías una copia del dato, sino la dirección de memoria donde vive la variable original. Esto significa que la función tiene acceso directo al dato real. Cualquier cambio que haga la función afectará permanentemente a la variable original.

**Ejemplo:**

<img width="812" height="461" alt="image" src="https://github.com/user-attachments/assets/cce9be32-d298-401f-860b-594a31d744a1" />

## Arreglos (Arrays)
Un arreglo es una estructura de datos que te permite almacenar una colección de elementos del mismo tipo (por ejemplo, una lista de puros números enteros, o puros textos) bajo un solo nombre de variable. Los datos se guardan en posiciones de memoria contiguas y se accede a ellos a través de un índice, el cual casi siempre comienza en 0.

Existen dos categorías principales:
### 1. Arreglos Unidimensionales (Vectores)
Es una estructura lineal, similar a una lista de elementos acomodados en una sola fila o columna.

**Ejemplo:**

<img width="788" height="272" alt="image" src="https://github.com/user-attachments/assets/6354e920-a6ec-428a-8a53-ee9a4d5a3680" />

### 2. Arreglos Bidimensionales (Matrices)
Son "arreglos de arreglos". El caso más común es el arreglo bidimensional, que funciona exactamente como una tabla o cuadrícula de Excel, estructurada en filas y columnas.

**Ejemplo:**

<img width="582" height="343" alt="image" src="https://github.com/user-attachments/assets/7ece8e41-1e74-4c2e-8c9e-2da1e28ecac5" />

### 3. Arreglos Tridimensionales
Un arreglo tridimensional añade una dimensión más a la matriz, lo que significa que es un "arreglo de matrices".

Si un arreglo unidimensional es una línea y un bidimensional es una tabla plana (filas y columnas), el tridimensional añade profundidad (o capas).

**Ejemplo:**

<img width="811" height="676" alt="image" src="https://github.com/user-attachments/assets/05eabc59-8dcf-4163-9369-dc323d4a1deb" />


## Principales dificultades y reflexión crítica
Mi unica dificultad en este trabajo fue tratar de analizar y comprender mejor las modularidades, pues se me dificultaba entender la diferencia entre ambos y que hace cada uno, pero ahora lo entiendo mejor y puedo estimar que las modularidades y los arreglos son muy esensiales en la programacion, pues nos pueden ayudar a simplicar trabajos y codigos, facilitando mas el trabajo a las computadoras y mejorar la comprencion del codigo mismo.
