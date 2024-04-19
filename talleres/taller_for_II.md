<div>
<h1 align="center">Taller: Explorando Ciclos For Anidados</h1>
</div>

Bienvenidos al taller avanzado sobre ciclos `for`, donde daremos un paso más allá en nuestra comprensión y uso de esta estructura de control fundamental en programación. En este taller, nos centraremos en los ciclos `for` anidados, una herramienta poderosa que permite manejar situaciones más complejas como el procesamiento de datos multidimensionales, la realización de cálculos iterativos complejos, y la simulación de escenarios que requieren múltiples niveles de decisión.

**Un ciclo `for` anidado ocurre cuando un ciclo `for` se coloca dentro de otro ciclo `for`**. Esta estructura es especialmente útil cuando necesitamos trabajar con matrices, tablas, o cualquier tipo de datos que se puedan representar como colecciones de colecciones. También son ideales para realizar operaciones que requieren comparar elementos entre sí, como ordenar o buscar patrones.

# Ejercicio 1
Analiza y determina qué realiza el siguiente algoritmo. Suponga que se tiene una lista de listas llamada `horario` que contiene las horas de estudio dedicadas a cinco asignaturas diferentes cada día de la semana (de lunes a viernes).

```
horario(5)  # Lista de listas, cada sublista representa un día con 5 horas de estudio para diferentes asignaturas

dia, asignatura, horas: Entero

Inicio

horas ← 0

Para dia ← 1 Hasta 5  # De lunes a viernes
    total_horas_dia ← 0
    
    Para asignatura ← 1 Hasta 5  # Cinco asignaturas diferentes
        total_horas_dia ← total_horas_dia + horario[dia][asignatura]
    Fin_para
    
    Si total_horas_dia > horas entonces
        horas ← total_horas_dia
    Fin_si
    
Fin_para

Imprimir horas

Fin
```

**¿Qué determina la ejecución de este algoritmo?**

	a. Calcula y muestra el total de horas de estudio por día.
	b. Muestra las horas dedicadas a la asignatura con más horas de estudio cada día.
	c. Calcula y muestra el día con el máximo total de horas de estudio.
	d. Imprime el total acumulado de horas de estudio de la semana.

# Ejercicio 2
Para el siguiente programa en Python, escriba los elementos que se imprimen en el orden específico:

```python
A = [[1, 2, 3], [4, 5, 6]]
B = [[5, 2, 1], [3, 10, 8]]

for i in range(2):
    for j in range(3):
        for k in range(2):
            for n in range(3):
                if A[i][j] == B[k][n]:
                    print(A[i][j])
```

**¿Qué elementos imprime este programa en el orden en que aparecen?**

	a. 5, 3, 2, 1
	b. 1, 4, 5, 6
	c. 1, 2, 3, 5
	d. 1, 2, 3, 4, 5, 6, 8, 10

# Ejercicio 3
Analiza y determina qué realiza el siguiente algoritmo. Suponga que se tienen dos listas, `lista1` y `lista2`, cada una con 100 elementos.

```
Entero M, N
Entero lista1(M), lista2(N)

Inicio

M ← 100
N ← 100

Para i ← 1 Hasta M
    Para j ← 1 Hasta N
        Si lista1[i] = lista2[j] Entonces
            Imprimir lista1[i], "lista1:" i, "lista2:", j
        Fin_si
    Fin_para
Fin_para

Fin
```
**¿Qué determina la ejecución de este algoritmo?**

	a. Suma los elementos coincidentes entre lista1 y lista2.
	b. Encuentra los elementos coincidentes entre lista1 y lista2 y muestra sus valores.
	c. Encuentra los elementos coincidentes entre lista1 y lista2 y reporta sus posiciones en ambas listas.
	d. Cuenta el número de coincidencias entre lista1 y lista2.

# Ejercicio 4

Considere el siguiente pseudocódigo y determine el contenido de la segunda lista interna al terminar el algoritmo, dado que las listas internas se actualizan con un procedimiento específico.


```
Variables:
    Entero: fil, col, i, j, k ← 0
    Lista: matriz

Inicio
    Escribir("Ingrese el número de elementos de matriz: ")
    Leer(fil)
    Escribir("Ingrese el número de elementos que tendrán las listas que componen a matriz: ")
    Leer(col)
    
    Para i ← 1 hasta fil haga
        matriz Agregar Lista nueva con 'col' ceros
    Fin_para
    
    # Actualizar los valores en la matriz
    Para j ← 1 hasta col haga
        Para i ← 1 hasta fil haga
            matriz[i][j] ← i^2 + k
            k ← k + 1
        Fin_para
    Fin_para
    Escribir(matriz)
Fin
```
**Si el usuario ingresa el número 3 para filas y 2 para columnas, ¿cuál será el contenido de la segunda lista interna al terminar el algoritmo?**

	A. [1, 2]
	B. [4, 5]
	C. [5, 8]
	D. [1, 4]

## Explicación
Para explicar y determinar el contenido de la segunda lista interna de la matriz al finalizar este algoritmo, primero vamos a repasar cómo se construye y se actualiza la matriz paso a paso, considerando los inputs de 3 para las filas (`fil`) y 2 para las columnas (`col`).

### Proceso de inicialización y actualización
1. **Inicialización de la Matriz**:
    - El usuario ingresa `3` para `fil` y `2` para `col`.
    - Se crea una matriz de `3` listas (filas), cada una conteniendo inicialmente `2` ceros.
    - Estado inicial de `matriz`: `[[0, 0], [0, 0], [0, 0]]`.
2. **Actualización de los Valores**:
    - El algoritmo procede a llenar la matriz utilizando dos bucles anidados que recorren las columnas (`col`) y luego las filas (`fil`).
    - La expresión `matriz[i][j] ← i^2 + k` indica que cada elemento de la matriz se actualiza con el cuadrado del índice de fila más el contador `k`, que se incrementa en cada paso.
    - Se considera que los índices `i` y `j` empiezan en 1, lo que es común en pseudocódigo pero puede ser confuso al traducirlo directamente a lenguajes como Python donde los índices comienzan en 0.

### Cálculo paso a paso
- **Primera Iteración de Columnas (`j = 1`)**:
    
    - **Para `i = 1`**: 12+0=112+0=1; `matriz[1][1] = 1`, $k$=1
    - **Para `i = 2`**: 22+1=522+1=5; `matriz[2][1] = 5`, $k$=2
    - **Para `i = 3`**: 32+2=1132+2=11; `matriz[3][1] = 11`, $k$=3
    - Estado de `matriz` después de `j = 1`: `[[0, 1], [0, 5], [0, 11]]`
- **Segunda Iteración de Columnas (`j = 2`)**:
    
    - **Para `i = 1`**: 12+3=412+3=4; `matriz[1][2] = 4`, $k$=4
    - **Para `i = 2`**: 22+4=822+4=8; `matriz[2][2] = 8`, $k$=5
    - **Para `i = 3`**: 32+5=1432+5=14; `matriz[3][2] = 14`, $k$=6
    - Estado final de `matriz`: `[[1, 4], [5, 8], [11, 14]]`

### Respuesta:
Dado que se pregunta por el contenido de la segunda lista interna al final del algoritmo, y basándonos en el cálculo detallado, la segunda lista interna de la matriz es `[5, 8]`. Por lo tanto, la respuesta correcta es:

C. [5, 8]

Esta opción corresponde a los valores calculados para la segunda fila después de completar las actualizaciones según las instrucciones del algoritmo proporcionado.

# Ejercicio 5
Considere el siguiente pseudocódigo y determine el contenido de la primera lista interna al terminar el algoritmo, dado que las listas internas se actualizan con un procedimiento específico.

```
Variables:
    Entero: fil, col, i, j, k ← 0
    Lista: matriz

Inicio
    Escribir("Ingrese el número de elementos de matriz: ")
    Leer(fil)
    Escribir("Ingrese el número de elementos que tendrán las listas que componen a matriz: ")
    Leer(col)
    
    Para i ← 1 hasta fil haga
        matriz Agregar Lista nueva con 'col' ceros
    Fin_para
    
    # Actualizar los valores en la matriz
    Para j ← 1 hasta col haga
        Para i ← 1 hasta fil haga
            matriz[i][j] ← 3*i + k
            k ← k + 2
        Fin_para
    Fin_para
    Escribir(matriz)
Fin
```
**Si el usuario ingresa el número 3 para filas y 2 para columnas, ¿cuál será el contenido de la primera lista interna al terminar el algoritmo?**

	A. [3, 11]
	B. [3, 9]
	C. [5, 13]
	D. [1, 7]

## Explicación del pseudocódigo y solución:

1. **Inicialización de la Matriz**:
    - El usuario ingresa `3` para `fil` y `2` para `col`.
    - Se crea una matriz con `3` listas internas (filas), cada una inicialmente conteniendo `2` ceros.
    - Estado inicial de `matriz`: `[[0, 0], [0, 0], [0, 0]]`.
2. **Actualización de los Valores**:
    - Los bucles anidados recorren las columnas y filas para actualizar los valores.
    - Cada valor en la matriz se calcula como `3*i + k`, y luego se incrementa `k` en 2 después de cada asignación.

### Cálculo paso a paso para la actualización:

- **Primera Iteración de Columnas (`j = 1`)**:
    
    - **Para `i = 1`**: 3∗1+0=33∗1+0=3; `matriz[1][1] = 3`, k=2
    - **Para `i = 2`**: 3∗2+2=83∗2+2=8; `matriz[2][1] = 8`, k=4
    - **Para `i = 3`**: 3∗3+4=133∗3+4=13; `matriz[3][1] = 13`, k=6
    - Estado intermedio de `matriz`: `[[3, 0], [8, 0], [13, 0]]`
- **Segunda Iteración de Columnas (`j = 2`)**:
    
    - **Para `i = 1`**: 3∗1+6=93∗1+6=9; `matriz[1][2] = 9`, k=8
    - **Para `i = 2`**: 3∗2+8=143∗2+8=14; `matriz[2][2] = 14`, k=10
    - **Para `i = 3`**: 3∗3+10=193∗3+10=19; `matriz[3][2] = 19`, k=12
    - Estado final de `matriz`: `[[3, 9], [8, 14], [13, 19]]`

### Respuesta:

El contenido de la primera lista interna al final del algoritmo es `[3, 9]`. Por lo tanto, la respuesta correcta es:

B. [3, 9]
