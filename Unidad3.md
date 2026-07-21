[<< Regresar al indice](https://github.com/AndyBlox208/PortafolioDigital/blob/main/Encabezado.md)

[<< Unidad 2](Unidad2.md)
# Unidad 3
## Modularidad
La modularidad es el principio de dividir un programa grande y complejo en fragmentos más pequeños, independientes y enfocados en una sola tarea. A estos fragmentos los llamamos módulos (también conocidos como funciones, métodos o procedimientos).

Diseñar el código de esta manera evita la repetición, facilita encontrar errores y permite que varios programadores trabajen en el mismo proyecto sin estorbarse.

Cuando el programa principal necesita usar un módulo, le envía información a través de parámetros. Existen dos formas de enviar esta información:
### 1. Pase de parámetro por valor
Cuando pasas un parámetro por valor, el programa le entrega a la función una copia exacta de la variable original. Si la función modifica ese dato, solo está alterando su copia local; la variable original permanece intacta.

**Ejemplo:**

En este ejemplo, usamos el pase por valor para calcular una predicción. Queremos saber cuánto dinero tendríamos en un año si aplicamos un 5% de interés, pero sin modificar el saldo real de nuestra cuenta todavía.

<img width="732" height="482" alt="image" src="https://github.com/user-attachments/assets/b55fb5f2-dabc-4ae6-a9eb-d4254392cf4a" />
<img width="600" height="93" alt="image" src="https://github.com/user-attachments/assets/86959d6c-d715-418c-8afb-c00dde828a0a" />

### 2. Pase de parámetro por referencia
Cuando pasas un parámetro por referencia, no envías una copia del dato, sino la dirección de memoria donde vive la variable original. Esto significa que la función tiene acceso directo al dato real. Cualquier cambio que haga la función afectará permanentemente a la variable original.

**Ejemplo:**

Aquí usamos punteros (referencia en C) para actualizar la posición de un objeto en movimiento. Al pasar la dirección de memoria, la función aplica la fórmula de Movimiento Rectilíneo Uniforme y altera permanentemente la variable original.

<img width="801" height="507" alt="image" src="https://github.com/user-attachments/assets/269ae949-f623-4db8-b551-dc1ca21aefd4" />
<img width="600" height="93" alt="image" src="https://github.com/user-attachments/assets/fc5f21b9-1363-4a26-90ce-34243abbc16c" />

## Arreglos (Arrays)
Un arreglo es una estructura de datos que te permite almacenar una colección de elementos del mismo tipo (por ejemplo, una lista de puros números enteros, o puros textos) bajo un solo nombre de variable. Los datos se guardan en posiciones de memoria contiguas y se accede a ellos a través de un índice, el cual casi siempre comienza en 0.

Existen dos categorías principales:
### 1. Arreglos Unidimensionales (Vectores)
Es una estructura lineal, similar a una lista de elementos acomodados en una sola fila o columna.

**Ejemplo:**

Usaremos un vector para almacenar los datos históricos de ventas y predecir el próximo mes utilizando un cálculo de promedio móvil simple.

<img width="817" height="436" alt="image" src="https://github.com/user-attachments/assets/ce7771d2-133a-44a8-b25f-2f07a72dbdaa" />
<img width="601" height="65" alt="image" src="https://github.com/user-attachments/assets/172acdec-a10f-46de-8243-4bbdc7571915" />

### 2. Arreglos Bidimensionales (Matrices)
Son "arreglos de arreglos". El caso más común es el arreglo bidimensional, que funciona exactamente como una tabla o cuadrícula de Excel, estructurada en filas y columnas.

**Ejemplo:**

Una matriz que representa la producción de dos fábricas diferentes durante un trimestre. Haremos un cálculo para sumar el rendimiento total de una fábrica específica.

<img width="755" height="491" alt="image" src="https://github.com/user-attachments/assets/8b27a6d5-081f-41b6-91ba-ae60746eef73" />
<img width="600" height="75" alt="image" src="https://github.com/user-attachments/assets/ceeb0793-11eb-44dc-a77f-06ec1620ec46" />

### 3. Arreglos Tridimensionales
Un arreglo tridimensional añade una dimensión más a la matriz, lo que significa que es un "arreglo de matrices".

Si un arreglo unidimensional es una línea y un bidimensional es una tabla plana (filas y columnas), el tridimensional añade profundidad (o capas).

**Ejemplo:**

El cubo de datos almacenará temperaturas. Las dimensiones serán: años, meses y días. Calcularemos la temperatura promedio de un mes específico dentro de un año específico.

<img width="745" height="726" alt="image" src="https://github.com/user-attachments/assets/c587ac11-4809-4e74-94d1-3e3a5cca4819" />
<img width="600" height="71" alt="image" src="https://github.com/user-attachments/assets/3be249cb-0b7a-443e-ac73-340567fcfa14" />

## Principales dificultades y reflexión crítica
Mi unica dificultad en este trabajo fue tratar de analizar y comprender mejor las modularidades, pues se me dificultaba entender la diferencia entre ambos y que hace cada uno, pero ahora lo entiendo mejor y puedo estimar que las modularidades y los arreglos son muy esensiales en la programacion, pues nos pueden ayudar a simplicar trabajos y codigos, facilitando mas el trabajo a las computadoras y mejorar la comprencion del codigo mismo.
