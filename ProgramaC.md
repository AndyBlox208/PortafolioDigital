<div align="center">
    
# Codificación y Validación del programa

</div>

## Código en C

```c
#include <stdio.h>
// Definimos las dimensiones de las matrices
#define FILAS 2
#define COLUMNAS 3
// Prototipos de las funciones
void completarMatrices(int matriz1[FILAS][COLUMNAS], int matriz2[FILAS][COLUMNAS]);
void sumaMatriz(int matriz1[FILAS][COLUMNAS], int matriz2[FILAS][COLUMNAS], int resultado[FILAS][COLUMNAS]);
void restaMatriz(int matriz1[FILAS][COLUMNAS], int matriz2[FILAS][COLUMNAS], int resultado[FILAS][COLUMNAS]);
void multiplicacionMatriz(int matriz1[FILAS][COLUMNAS], int matriz2[FILAS][COLUMNAS], int resultado[FILAS][COLUMNAS]);
void mostrarResultado(const char* nombreOperacion, int matriz[FILAS][COLUMNAS]);
// Función main: Solo declara variables y llama a las demás funciones
int main() {
    // Declaración de las matrices
    int matrizA[FILAS][COLUMNAS];
    int matrizB[FILAS][COLUMNAS];
    int matrizResultado[FILAS][COLUMNAS];
    printf("--- OPERACIONES CON MATRICES 2x3 ---\n\n");
    // Llenar las matrices
    completarMatrices(matrizA, matrizB);
    // Suma
    sumaMatriz(matrizA, matrizB, matrizResultado);
    mostrarResultado("Suma (A + B)", matrizResultado);
    // Resta
    restaMatriz(matrizA, matrizB, matrizResultado);
    mostrarResultado("Resta (A - B)", matrizResultado);
    // Multiplicación
    multiplicacionMatriz(matrizA, matrizB, matrizResultado);
    // Resultados
    mostrarResultado("Multiplicacion (A * B)", matrizResultado);
    return 0;
}
// Función completarMatrices: Pide al usuario que ingrese los datos
void completarMatrices(int matriz1[FILAS][COLUMNAS], int matriz2[FILAS][COLUMNAS]) {
    printf("Ingrese los valores para la Matriz A (2x3):\n");
    for (int i=0; i<FILAS; i++) {
        for (int j=0; j<COLUMNAS; j++) {
            printf("Matriz A [%d][%d]: ", i, j);
            scanf("%d", &matriz1[i][j]);
        }
    }
    printf("\nIngrese los valores para la Matriz B (2x3):\n");
    for (int i=0; i<FILAS; i++) {
        for (int j=0; j<COLUMNAS; j++) {
            printf("Matriz B [%d][%d]: ", i, j);
            scanf("%d", &matriz2[i][j]);
        }
    }
}
// Función sumaMatriz: Suma posiciones correspondientes
void sumaMatriz(int matriz1[FILAS][COLUMNAS], int matriz2[FILAS][COLUMNAS], int resultado[FILAS][COLUMNAS]) {
    for (int i=0; i<FILAS; i++) {
        for (int j=0; j<COLUMNAS; j++) {
            resultado[i][j] = matriz1[i][j] + matriz2[i][j];
        }
    }
}
// Función restaMatriz: Resta posiciones correspondientes
void restaMatriz(int matriz1[FILAS][COLUMNAS], int matriz2[FILAS][COLUMNAS], int resultado[FILAS][COLUMNAS]) {
    for (int i=0; i<FILAS; i++) {
        for (int j=0; j<COLUMNAS; j++) {
            resultado[i][j] = matriz1[i][j] - matriz2[i][j];
        }
    }
}
// Función multiplicacionMatriz: Multiplica posiciones correspondientes
void multiplicacionMatriz(int matriz1[FILAS][COLUMNAS], int matriz2[FILAS][COLUMNAS], int resultado[FILAS][COLUMNAS]) {
    for (int i=0; i<FILAS; i++) {
        for (int j=0; j<COLUMNAS; j++) {
            resultado[i][j] = matriz1[i][j] * matriz2[i][j];
        }
    }
}
// Función mostrarResultado: Imprime la matriz en formato de cuadrícula
void mostrarResultado(const char* nombreOperacion, int matriz[FILAS][COLUMNAS]) {
    printf("\n--- Resultado de la %s ---\n", nombreOperacion);
    for (int i=0; i<FILAS; i++) {
        for (int j=0; j<COLUMNAS; j++) {
            printf("%d\t", matriz[i][j]); // \t tabula los números para que se vean como tabla
        }
        printf("\n");
    }
}
```
## Casos de prueba

<img width="583" height="663" alt="image" src="https://github.com/user-attachments/assets/2e16f7b8-5dd7-41f1-87ad-4f1ce6d64047" />
