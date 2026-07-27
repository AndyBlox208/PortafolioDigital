<div align="center">
    
# Codificación y Validación del programa en Java

</div>

## Código en Java

```java
import java.util.Scanner;

public class ApeMatrizJava {

    // Definimos las dimensiones de las matrices
    static final int FILAS = 2;
    static final int COLUMNAS = 3;

    // Función main: Solo declara variables y llama a las demás funciones
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Declaración de las matrices
        int[][] matrizA = new int[FILAS][COLUMNAS];
        int[][] matrizB = new int[FILAS][COLUMNAS];
        int[][] matrizResultado = new int[FILAS][COLUMNAS];

        System.out.println("--- OPERACIONES CON MATRICES 2x3 ---\n");

        // Llenar las matrices
        completarMatrices(scanner, matrizA, matrizB);

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

        scanner.close();
    }

    // Función completarMatrices: Pide al usuario que ingrese los datos
    public static void completarMatrices(Scanner scanner, int[][] matriz1, int[][] matriz2) {
        System.out.println("Ingrese los valores para la Matriz A (2x3):");
        for (int i = 0; i < FILAS; i++) {
            for (int j = 0; j < COLUMNAS; j++) {
                System.out.printf("Matriz A [%d][%d]: ", i, j);
                matriz1[i][j] = scanner.nextInt();
            }
        }

        System.out.println("\nIngrese los valores para la Matriz B (2x3):");
        for (int i = 0; i < FILAS; i++) {
            for (int j = 0; j < COLUMNAS; j++) {
                System.out.printf("Matriz B [%d][%d]: ", i, j);
                matriz2[i][j] = scanner.nextInt();
            }
        }
    }

    // Función sumaMatriz: Suma posiciones correspondientes
    public static void sumaMatriz(int[][] matriz1, int[][] matriz2, int[][] resultado) {
        for (int i = 0; i < FILAS; i++) {
            for (int j = 0; j < COLUMNAS; j++) {
                resultado[i][j] = matriz1[i][j] + matriz2[i][j];
            }
        }
    }

    // Función restaMatriz: Resta posiciones correspondientes
    public static void restaMatriz(int[][] matriz1, int[][] matriz2, int[][] resultado) {
        for (int i = 0; i < FILAS; i++) {
            for (int j = 0; j < COLUMNAS; j++) {
                resultado[i][j] = matriz1[i][j] - matriz2[i][j];
            }
        }
    }

    // Función multiplicacionMatriz: Multiplica posiciones correspondientes
    public static void multiplicacionMatriz(int[][] matriz1, int[][] matriz2, int[][] resultado) {
        for (int i = 0; i < FILAS; i++) {
            for (int j = 0; j < COLUMNAS; j++) {
                resultado[i][j] = matriz1[i][j] * matriz2[i][j];
            }
        }
    }

    // Función mostrarResultado: Imprime la matriz en formato de cuadrícula
    public static void mostrarResultado(String nombreOperacion, int[][] matriz) {
        System.out.printf("\n--- Resultado de la %s ---\n", nombreOperacion);
        for (int i = 0; i < FILAS; i++) {
            for (int j = 0; j < COLUMNAS; j++) {
                System.out.print(matriz[i][j] + "\t"); // \t tabula los números para que se vean como tabla
            }
            System.out.println();
        }
    }
}
```
## Casos de prueba en Java

<img width="633" height="663" alt="image" src="https://github.com/user-attachments/assets/1d3170bd-6148-42d3-8ef8-30164cb5defc" />
