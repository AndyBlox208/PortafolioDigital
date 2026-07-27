<div align="center">
    
# Codificación y Validación del programa en Python

</div>

## Código en Python

```python
# Definimos las dimensiones de las matrices
FILAS = 2
COLUMNAS = 3

def completar_matrices():
    """Pide al usuario que ingrese los datos para ambas matrices y las retorna."""
    matriz1 = [[0] * COLUMNAS for _ in range(FILAS)]
    matriz2 = [[0] * COLUMNAS for _ in range(FILAS)]
    
    print("Ingrese los valores para la Matriz A (2x3):")
    for i in range(FILAS):
        for j in range(COLUMNAS):
            matriz1[i][j] = int(input(f"Matriz A [{i}][{j}]: "))
            
    print("\nIngrese los valores para la Matriz B (2x3):")
    for i in range(FILAS):
        for j in range(COLUMNAS):
            matriz2[i][j] = int(input(f"Matriz B [{i}][{j}]: "))
            
    return matriz1, matriz2

def suma_matriz(matriz1, matriz2):
    """Suma posiciones correspondientes."""
    resultado = [[0] * COLUMNAS for _ in range(FILAS)]
    for i in range(FILAS):
        for j in range(COLUMNAS):
            resultado[i][j] = matriz1[i][j] + matriz2[i][j]
    return resultado

def resta_matriz(matriz1, matriz2):
    """Resta posiciones correspondientes."""
    resultado = [[0] * COLUMNAS for _ in range(FILAS)]
    for i in range(FILAS):
        for j in range(COLUMNAS):
            resultado[i][j] = matriz1[i][j] - matriz2[i][j]
    return resultado

def multiplicacion_matriz(matriz1, matriz2):
    """Multiplica posiciones correspondientes (producto elemento a elemento)."""
    resultado = [[0] * COLUMNAS for _ in range(FILAS)]
    for i in range(FILAS):
        for j in range(COLUMNAS):
            resultado[i][j] = matriz1[i][j] * matriz2[i][j]
    return resultado

def mostrar_resultado(nombre_operacion, matriz):
    """Imprime la matriz en formato de cuadrícula."""
    print(f"\n--- Resultado de la {nombre_operacion} ---")
    for i in range(FILAS):
        for j in range(COLUMNAS):
            # \t tabula los números para que se vean como tabla
            print(f"{matriz[i][j]}\t", end="") 
        print()

def main():
    print("--- OPERACIONES CON MATRICES 2x3 ---\n")
    
    # Llenar las matrices
    matrizA, matrizB = completar_matrices()
    
    # Suma
    matriz_resultado = suma_matriz(matrizA, matrizB)
    mostrar_resultado("Suma (A + B)", matriz_resultado)
    
    # Resta
    matriz_resultado = resta_matriz(matrizA, matrizB)
    mostrar_resultado("Resta (A - B)", matriz_resultado)
    
    # Multiplicación
    matriz_resultado = multiplicacion_matriz(matrizA, matrizB)
    
    # Resultados
    mostrar_resultado("Multiplicacion (A * B)", matriz_resultado)

# Equivalente al 'int main()' de C para ejecutar el script
if __name__ == "__main__":
    main()
```
## Casos de prueba en Python

<img width="922" height="732" alt="image" src="https://github.com/user-attachments/assets/6f67f977-831f-416f-bc97-ad3ee786a0f9" />
