<h1>2323 - FUNDAMENTOS DE PROGRAMACION -- UEA-L-UFB-026</h1>

<h3>Repositorio de código fuente utilizado en la Asignatura Fundamentos de Programación</h3>

<p>
    <strong>Institución: </strong>Universidad Estatal Amazónica <br>
    <strong>Carrera: </strong>Ingeniería en Tecnologías de la Información y Comunicación <br>
    <strong>Docente: </strong>Ing. Edwin Gustavo Fernández Sánchez, Mgs. <br>
</p>
# Programa 1: Búsqueda en Arreglo Multidimensional

# Definición de la matriz
matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]

# Función para búsqueda en la matriz
def buscar_valor(matriz, valor):
    for i in range(len(matriz)):
        for j in range(len(matriz[i])):
            if matriz[i][j] == valor:
                return True, i, j
    return False, None, None

# Valor a buscar
valor_buscar = 5

# Realizar la búsqueda
encontrado, fila, columna = buscar_valor(matrix, valor_buscar)

# Mostrar resultado
if encontrado:
    print(f"El valor {valor_buscar} se encontró en la posición ({fila}, {columna})")
else:
    print(f"El valor {valor_buscar} no se encontró en la matriz.")
