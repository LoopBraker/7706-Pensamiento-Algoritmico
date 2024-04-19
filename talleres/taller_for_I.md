<div>
<h1 align="center">Taller</h1>
</div>

Bienvenidos al taller donde exploraremos el poder y la flexibilidad del ciclo for en la programación. Este taller está diseñado para ayudaros a familiarizaros con el uso básico del ciclo `for`, un componente esencial en la mayoría de los lenguajes de programación. El objetivo es comprender cómo utilizar este tipo de bucle para iterar sobre estructuras de datos y realizar operaciones repetitivas de manera eficiente.

Un ciclo for se utiliza para repetir un bloque de código un número específico de veces, lo que lo hace ideal para operaciones como procesar elementos en una lista, realizar cálculos repetitivos, o simplemente repetir una acción hasta que se cumpla una condición.

En este taller, nos centraremos exclusivamente en ejercicios que involucran un único ciclo `for`, sin utilizar ciclos anidados. Esto nos permitirá concentrarnos en entender cada aspecto del ciclo for sin las complicaciones adicionales que introducen los bucles múltiples.

# Ejercicio 1
Determina qué realiza el siguiente algoritmo. Suponga que la lista `ventas` ya está creada y contiene los registros de ventas de un producto durante 30 días.

```pseudocode
ventas(30)
k, a: Entero

Inicio

a ← 0

Para k ← 1 Hasta 30
    Si ventas[k] > a entonces
        a ← ventas[k]
    Fin si
Fin_para

Imprimir a

Fin 
```

**¿Qué determina la ejecución de este algoritmo?**

	a. Muestra la posición del elemento mayor de la lista.
	b. Muestra el elemento mayor de la lista.
	c. Muestra las ventas del producto en los 30 días.
	d. Imprime el valor inicial de `a`.

# Ejercicio 2
Analiza y determina qué realiza el siguiente algoritmo. Suponga que la lista `ventas` ya está creada y contiene los registros de ventas de un producto durante 30 días.

```pseudocode
ventas(30)
k, s: Entero

Inicio

s ← 0

Para k ← 1 Hasta 30
    s ← s + ventas[k]
Fin_para

Imprimir s

Fin
```

**¿Qué determina la ejecución de este algoritmo?**

	a. Muestra la posición del elemento mayor de la lista.
	b. Muestra el elemento mayor de la lista.
	c. Muestra la suma total de las ventas en los 30 días.
	d. Imprime el valor inicial de `s`.

# Ejercicio 3
Analiza y determina qué realiza el siguiente algoritmo. Suponga que la lista `temperaturas` ya está creada y contiene las temperaturas máximas registradas cada día durante un mes de 30 días.

```pseudocode
temperaturas(30)
k, x, y: Real

Inicio

x ← 0.0

Para k ← 1 Hasta 30
    x ← x + temperaturas[k]
Fin_para

y ← x / 30

Imprimir y

Fin

```

**¿Qué determina la ejecución de este algoritmo?**

	a. Muestra la temperatura máxima registrada en el mes.
	b. Muestra la temperatura mínima registrada en el mes.
	c. Calcula y muestra el promedio mensual de las temperaturas.
	d. Imprime la suma total de las temperaturas del mes.

# Ejercicio 4
Analiza y determina qué realiza el siguiente algoritmo. Suponga que la lista `puntuaciones` ya está creada y contiene los resultados de 10 exámenes de un estudiante durante un semestre.

```pseudocode
puntuaciones(10)
k, c: Entero

Inicio

c ← 0

Para k ← 1 Hasta 10
    Si puntuaciones[k] >= 75 entonces
        c ← c + 1
    Fin si
Fin_para

Imprimir c

Fin
```

**¿Qué determina la ejecución de este algoritmo?**

	a. Calcula y muestra la cantidad de exámenes en los que el estudiante obtuvo al menos 75 puntos.
	b. Muestra el promedio de las puntuaciones de los exámenes.
	c. Muestra el total de puntos obtenidos en los exámenes.
	d. Imprime el número de exámenes tomados.

# Ejercicio 5
Determina qué realiza el siguiente algoritmo. Suponga que la lista `lista_numeros` ya está creada y contiene 1000 elementos.

```pseudocode
Entero M, X, R
Entero lista_numeros(M)

Inicio

M ← 1000
X ← 0 , R ← 0

Para I ← 1 Hasta M
    Si lista_numeros[I] > 0 Entonces
        X ← X + lista_numeros[I]
    Sino
        R ← R + 1
    Fin_si
Fin_para

Imprimir X, R

Fin
```

**¿Qué determina la ejecución de este algoritmo?**

	a. Suma los números pares y cuenta los números impares de la lista.
	b. Suma los números negativos y cuenta los números positivos de la lista.
	c. Suma los números positivos y los números negativos de la lista.
	d. Suma los números positivos y cuenta los números negativos de la lista.

# Ejercicio 6
Pregunta: Analiza y determina qué realiza el siguiente algoritmo. Suponga que la lista `datos` ya está creada y contiene 100 elementos.

```pseudocode
Entero M, D, T
Entero datos(M)

Inicio

M ← 100
D ← 0

Para i ← 1 Hasta M-1
    T ← datos[i+1] - datos[i]
    Si T > D Entonces
        D ← T
    Fin_si
Fin_para

Imprimir "El valor máximo de T es:", D

Fin
```

**¿Qué determina la ejecución de este algoritmo?**

	a. Encuentra y muestra la menor diferencia entre dos elementos consecutivos en la lista.
	b. Encuentra y muestra la mayor suma entre dos elementos consecutivos en la lista.
	c. Encuentra y muestra la mayor diferencia entre dos elementos consecutivos en la lista.
	d. Cuenta cuántas veces la diferencia entre dos elementos consecutivos es positiva.

# Ejercicio 7
Analiza y determina qué realiza el siguiente algoritmo. Suponga que la lista valores ya está creada y contiene 200 elementos.

```pseudocode
Entero M, V
Entero valores(M)

Inicio

M ← 200
V ← 0

Para i ← 1 Hasta M
    Si valores[i] < 0 Entonces
        V ← valores[i]
        Salir del Para
    Fin_si
Fin_para

Imprimir V

Fin
```

**¿Qué determina la ejecución de este algoritmo?**

	a. Encuentra y muestra el primer valor negativo en la lista.
	b. Suma todos los valores negativos en la lista y muestra el total.
	c. Cuenta y muestra la cantidad de valores negativos en la lista.
	d. Muestra el último valor negativo encontrado en la lista.

# Ejercicio 8
Analiza y determina qué realiza el siguiente algoritmo. Suponga que la lista elementos ya está creada y contiene 150 elementos.

```pseudocode
Entero M, S
Entero elementos(M)

Inicio

M ← 150
S ← 0

Para i ← 1 Hasta M
    Si elementos[i] < 0 Entonces
        Continuar
    Fin_si
    S ← S + elementos[i]
Fin_para

Imprimir "Suma de todos los valores no negativos:", S

Fin
```

**¿Qué determina la ejecución de este algoritmo?**

	a. Suma todos los valores en la lista y muestra el total.
	b. Encuentra y muestra el primer valor no negativo en la lista.
	c. Suma todos los valores no negativos en la lista y muestra el total.
	d. Cuenta y muestra la cantidad de valores negativos en la lista.

```python
elementos = [1, -1, 2, -2, 3, -3, 4,-5,7,10,-2]  # ejemplo con algunos valores, completa según sea necesario

S = 0

for i in elementos:
    if i < 0:
        continue  # Salta al próximo ciclo si el elemento es negativo
    S += elementos[i]

print("Suma de todos los valores no negativos:", S)
```

# Ejercicio 9
Considere el siguiente fragmento de código en Python y determine cuáles serán los valores finales del vector V:

```python
V = [0] * 8  # Crear una lista con 8 elementos inicializados a 0
V[0] = 2
V[1] = 5

for i in range(2, 8):  # Desde V[2] hasta V[7]
    if (i % 2) == 1:
        V[i] = V[i-1] + V[i-2]
    else:
        V[i] = V[i-1] % 2

print(V)  # Imprimir el vector resultante
```

**¿Cuáles son los valores finales en el vector V?**

	a) 2, 5, 7, 12, 19, 24, 31, 50
	b) 2, 5, 1, 6, 0, 6, 0, 6
	c) 2, 5, 7, 1, 2, 1, 2, 1
	d) Ninguna de las anteriores

## Explicación
1. **Inicialización de la lista `V`**:
    
    - `V = [0] * 8` crea una lista llamada `V` con 8 elementos, todos inicializados a 0. La lista `V` se verá así inicialmente: `[0, 0, 0, 0, 0, 0, 0, 0]`.
2. **Asignación de valores iniciales**:
    
    - `V[0] = 2` establece el primer elemento de la lista `V` en 2, por lo que ahora `V` se ve así: `[2, 0, 0, 0, 0, 0, 0, 0]`.
    - `V[1] = 5` establece el segundo elemento de la lista `V` en 5, cambiando `V` a: `[2, 5, 0, 0, 0, 0, 0, 0]`.
3. **Ciclo `for`**:
    
    - `for i in range(2, 8)` inicia un ciclo que comienza en 2 y termina en 7 (el rango en Python no incluye el límite superior, por lo que no llega hasta 8).
    - Dentro de este ciclo, se evalúan dos condiciones diferentes basadas en el índice `i`:
        - **Condición si `i` es impar (`if (i % 2) == 1`)**: Si el índice es impar (es decir, 3, 5, 7), la instrucción es `V[i] = V[i-1] + V[i-2]`. Esto significa que el elemento actual `V[i]` se establecerá como la suma de los dos elementos anteriores en la lista `V`.
        - **Condición si `i` es par (`else`)**: Si el índice es par (es decir, 2, 4, 6), la instrucción es `V[i] = V[i-1] % 2`. Esto establece `V[i]` como el resultado del módulo 2 del elemento anterior, lo que da 0 si el número es par y 1 si es impar.
4. **Impresión del resultado**:
    
    - `print(V)` imprime el contenido final de la lista `V` después de que todas las modificaciones se hayan realizado en el ciclo.

Veamos un desglose de cómo se modifica `V` en cada iteración del ciclo:

- Para `i = 2`: `V[2] = V[1] % 2 = 5 % 2 = 1` → `[2, 5, 1, 0, 0, 0, 0, 0]`
- Para `i = 3`: `V[3] = V[2] + V[1] = 1 + 5 = 6` → `[2, 5, 1, 6, 0, 0, 0, 0]`
- Para `i = 4`: `V[4] = V[3] % 2 = 6 % 2 = 0` → `[2, 5, 1, 6, 0, 0, 0, 0]`
- Para `i = 5`: `V[5] = V[4] + V[3] = 0 + 6 = 6` → `[2, 5, 1, 6, 0, 6, 0, 0]`
- Para `i = 6`: `V[6] = V[5] % 2 = 6 % 2 = 0` → `[2, 5, 1, 6, 0, 6, 0, 0]`
- Para `i = 7`: `V[7] = V[6] + V[5] = 0 + 6 = 6` → `[2, 5, 1, 6, 0, 6, 0, 6]`

El resultado final de `V` es `[2, 5, 1, 6, 0, 6, 0, 6]`, que muestra cómo cada operación basada en la paridad del índice afecta los valores almacenados en la lista.


# Ejercicio 10
Analiza y determina cuántas veces se ejecuta el ciclo for en el siguiente pseudocódigo antes de que se detenga:

```pseudocode
Inicio

s ← 30
cont1 ← 0
cont2 ← 0

Para i Desde 1 Hasta 100

    Si s <= 1 Entonces
        Salir del Para
    Fin_si
    
    Si (s Modulo 3 = 0) Entonces
        cont1 ← cont1 + 1
    Sino
        cont2 ← cont2 + 1
    Fin_si

    s ← s Dividido 2
    
Fin_Para

Imprimir cont1, cont2

Fin
```

**¿Cuántas veces se ejecuta el ciclo for antes de detenerse?**

	a) 10 veces
	b) 5 veces
	c) 4 veces
	d) Ninguna de las anteriores

# Ejercicio 11
Analiza y determina cuántas veces se ejecuta el ciclo for en el siguiente pseudocódigo antes de que se detenga (_Nota: considere que la lista inicia con el indice 0_):

```pseudocode
Inicio

T ← [15, 20, 25, 18, 12, 8, 10, 16, 20, 22, 5, 10]
u ← 10
cont ← 0

Para i Desde 1 Hasta 12
    Si T[i] < u Entonces
        Salir del Para
    Fin_si

    cont ← cont + 1
Fin_Para

Imprimir i
Imprimir cont

Fin
```

**¿Cuántas veces se ejecuta el ciclo for antes de detenerse?**

	a) 5 veces
	b) 6 veces
	c) 7 veces
	d) Ninguna de las anteriores

# Ejercicio 12
Considere el siguiente fragmento de código en Python y determine cuáles serán los valores finales del vector `W`:

```python
W = [0] * 10  # Crear una lista con 10 elementos inicializados a 0
W[0] = 3
W[1] = 4

for i in range(2, 10):  # Desde W[2] hasta W[9]
    if (i % 2) == 0:
        W[i] = W[i-1] + W[i-2]
    else:
        W[i] = W[i-1] * 2

    if W[i] > 20:
        W[i] = 10

print(W)  # Imprimir el vector resultante
```

**¿Cuáles son los valores finales en el vector W?**

	a) 3, 4, 7, 8, 15, 16, 31, 32, 63, 64
	b) 3, 4, 7, 8, 15, 30, 10, 20, 10, 20
	c) 3, 4, 7, 8, 15, 30, 10, 20, 10, 40
	d) Ninguna de las anteriores

### Explicación 

1. **Inicialización**:
    - Se comienza con `W = [3, 4, 0, 0, 0, 0, 0, 0, 0, 0]` después de asignar `W[0] = 3` y `W[1] = 4`.
1. **Iteraciones del ciclo `for`**:
    - `i = 2`: Es par, entonces `W[2] = W[1] + W[0] = 4 + 3 = 7`. La lista ahora es `[3, 4, 7, 0, 0, 0, 0, 0, 0, 0]`.
    - `i = 3`: Es impar, entonces `W[3] = W[2] * 2 = 7 * 2 = 14`. La lista se actualiza a `[3, 4, 7, 14, 0, 0, 0, 0, 0, 0]`.
    - `i = 4`: Es par, entonces `W[4] = W[3] + W[2] = 14 + 7 = 21`. Como `21 > 20`, se ajusta `W[4] = 10`. La lista cambia a `[3, 4, 7, 14, 10, 0, 0, 0, 0, 0]`.
    - `i = 5`: Es impar, entonces `W[5] = W[4] * 2 = 10 * 2 = 20`. La lista ahora es `[3, 4, 7, 14, 10, 20, 0, 0, 0, 0]`.
    - `i = 6`: Es par, entonces `W[6] = W[5] + W[4] = 20 + 10 = 30`. Como `30 > 20`, se ajusta `W[6] = 10`. La lista se actualiza a `[3, 4, 7, 14, 10, 20, 10, 0, 0, 0]`.
    - `i = 7`: Es impar, entonces `W[7] = W[6] * 2 = 10 * 2 = 20`. La lista cambia a `[3, 4, 7, 14, 10, 20, 10, 20, 0, 0]`.
    - `i = 8`: Es par, entonces `W[8] = W[7] + W[6] = 20 + 10 = 30`. Como `30 > 20`, se ajusta `W[8] = 10`. La lista ahora es `[3, 4, 7, 14, 10, 20, 10, 20, 10, 0]`.
    - `i = 9`: Es impar, entonces `W[9] = W[8] * 2 = 10 * 2 = 20`. La lista final es `[3, 4, 7, 14, 10, 20, 10, 20, 10, 20]`.
3. **Resultado Final**:
    - La lista final `W` es `[3, 4, 7, 14, 10, 20, 10, 20, 10, 20]`.

Por lo tanto, entre las opciones dadas, la correcta sería: _b) 3, 4, 7, 8, 15, 30, 10, 20, 10, 20_

# Ejercicio 13
Pregunta: Considere el siguiente algoritmo en pseudocódigo. Determine qué lista se imprimirá dado un número específico ingresado por el usuario.

```pseudocode
Variables:
    Entero: num, i
    Lista: d

Inicio
    Escribir("Ingrese un número: ")
    Leer(num)

    Para i ← 1 hasta num haga
        Si (num MODULO i) == 0 entonces
            Agregar i a d
        Fin_si
    Fin_para

    imprimir(d)
Fin
```

**Si el usuario ingresa el número 12, ¿cuál será el contenido de `d` al terminar el algoritmo?**

	a. 1, 2, 3, 4
	b. 1, 2, 3, 4, 6, 12
	c. 2, 3, 5, 6
	d. 2, 3, 4, 6

### Explicación del pseudocódigo:
- **Inicialización de variables**: Se define `num` para guardar el número ingresado por el usuario y `d` como una lista para almacenar los divisores del número.
- **Entrada del usuario**: El algoritmo solicita al usuario ingresar un número y lo guarda en `num`.
- **Bucle para encontrar divisores**: Se itera desde 1 hasta `num`. Para cada número `i`, si `i` es divisor de `num` (es decir, `num MODULO i` es 0), entonces `i` se agrega a la lista `d`.
- **Impresión de los divisores**: Al final del algoritmo, se imprime la lista `d` que contiene todos los divisores del número ingresado.

# Ejercicio 14

Pregunta: Considere el siguiente fragmento de código en Python para sumar los elementos de las posiciones pares en una lista `V` de `N` elementos con valores ya ingresados. Complete el espacio en blanco para que el algoritmo funcione correctamente.

```python
V = [2, 3, 5, 8, 13, 21]  # Ejemplo de lista con elementos ya ingresados.
N = len(V)
suma = 0

for i in range(N):
    if ______________:
        suma += V[i]

print("Suma de elementos en posiciones pares:", suma)
```

**Seleccione la opción que completa correctamente el algoritmo:**
	A. `i % 2 == 0`
	B. `V[i] % 2 == 0`
	C. `i // 2 == 0`
	D. `V[i] // 2 == 0`

## Explicación de la solución:

En Python, los índices de las listas comienzan en 0. Por lo tanto, los elementos en posiciones pares según la convención común (1, 3, 5,...) se encuentran en índices impares (0, 2, 4,...). La condición para seleccionar elementos en posiciones pares desde la perspectiva humana sería seleccionar elementos cuyo índice es impar.

- **Opción A**: `i % 2 == 0`. Esta condición verifica si el índice es par, lo que no es correcto según la pregunta, que pide sumar elementos en posiciones pares (índices impares).
- **Opción B**: `V[i] % 2 == 0`. Esta condición verifica si el elemento en la posición `i` es par, que no tiene relación con la posición del elemento.
- **Opción C**: `i // 2 == 0`. Esto se cumpliría solo cuando `i` es 0, lo que no es útil para sumar todos los elementos en posiciones pares.
- **Opción D**: `V[i] // 2 == 0`. Al igual que la B, verifica una propiedad del valor del elemento, no su posición.

La descripción y la explicación implican que queremos sumar elementos que están en posiciones como la segunda, cuarta, sexta, etc., que en la indexación de Python son 1, 3, 5, etc. Por tanto, la condición correcta en Python para sumar los elementos en posiciones pares, según la indexación basada en cero y el uso habitual del término "par" en este contexto, sería:

**A. `i % 2 == 0`** — Aunque parece contra-intuitiva debido a la descripción, en Python, esto seleccionaría índices 0, 2, 4, etc., los cuales corresponden a las primeras, terceras, quintas posiciones, etc., si empezamos a contar desde 1. Si la pregunta realmente intenta obtener los elementos en posiciones "pares" como segunda, cuarta, etc., desde un punto de vista humano (no técnico), entonces la condición correcta debería ser `i % 2 != 0`.

# Ejercicio 15

Pregunta: Considere el siguiente fragmento de código en Python para sumar los elementos que son mayores que un número dado y que se encuentran en posiciones impares en una lista `V` de `N` elementos. Complete el espacio en blanco para que el algoritmo funcione correctamente.

```python
V = [10, 20, 15, 25, 10, 30, 5, 40]  # Ejemplo de lista con elementos ya ingresados.
umbral = 18
suma = 0

for i in range(len(V)):
    if ______________:
        suma += V[i]

print("Suma de elementos mayores que", umbral, "en posiciones impares:", suma)
```

**Seleccione la opción que completa correctamente el algoritmo:**
	A. `i % 2 == 1 and V[i] > umbral`
	B. `i % 2 == 0 and V[i] > umbral`
	C. `i % 2 == 1 or V[i] > umbral`
	D. `i % 2 == 0 or V[i] > umbral`

## Explicación de la solución:

El objetivo es sumar los elementos que no solo son mayores que `umbral` sino que también están en posiciones impares de la lista, lo que significa que están en los índices 1, 3, 5, etc., dado que la indexación en Python comienza en 0.

- **Opción A**: `i % 2 == 1 and V[i] > umbral`. Esta opción es correcta porque `i % 2 == 1` selecciona los índices impares (posiciones "pares" si se comienza a contar desde 1), y `V[i] > umbral` asegura que solo se sumen los valores que excedan el umbral.
    
- **Opción B**: `i % 2 == 0 and V[i] > umbral`. Esta condición es incorrecta porque selecciona índices pares, que corresponden a posiciones impares si se comienza a contar desde 1, no cumpliendo el requisito de posiciones "impares".
    
- **Opción C**: `i % 2 == 1 or V[i] > umbral`. Es incorrecta porque el uso del `or` hace que la condición sea demasiado inclusiva, sumando elementos que son mayores que el umbral incluso si están en posiciones pares.
    
- **Opción D**: `i % 2 == 0 or V[i] > umbral`. También es incorrecta por el mismo motivo que la C, pero con una lógica inversa para la selección de índices.
    

Por lo tanto, la respuesta correcta es **A. `i % 2 == 1 and V[i] > umbral`**, ya que cumple con ambos requisitos del problema: seleccionar elementos en posiciones impares y que estos elementos sean mayores que el valor umbral establecido.

# Ejercicio 16
Considere el siguiente pseudocódigo y determine el valor de `i` al terminar la ejecución del algoritmo cuando se ingresa el valor `1`. _Nota: considere que los indices de lista inician en 1, no en 0_

```pseudocode
Variables:
    Entero: V = [4, 8, 90, 1, 78], n, i

Inicio
    Escribir("Ingrese un número a buscar: ")
    Leer(n)
    
    Para i ← 1 hasta 5 haga
        Si n = V[i] entonces
            Salir del Para
        Fin si
    Fin para
    
    Escribir("El valor de i es: ", i)
Fin
```

**Si se ingresa el número `1`, ¿cuál es el valor de `i` al terminar la ejecución del algoritmo?**

	A. 3
	B. 4
	C. 5
	D. El ciclo no termina

## Explicación de la solución:

El algoritmo inicializa una lista `V` con los valores `[4, 8, 90, 1, 78]`. Se solicita al usuario que ingrese un número `n` para buscar en la lista. El ciclo `para` itera sobre los elementos de la lista `V`, comenzando desde el índice 1 (suponiendo que el pseudocódigo se basa en una indexación que comienza desde 1, como es común en algunos lenguajes de programación de alto nivel y ejemplos educativos).

- **Proceso de búsqueda**:
    - El ciclo verifica cada elemento de `V` para ver si coincide con `n`.
    - Si se encuentra una coincidencia, el ciclo se rompe utilizando `Salir del Para`.

En el caso de que se ingrese el número `1`, el algoritmo buscará en `V` hasta encontrar este número. Dado que `1` está en la posición 4 de la lista `V`, el ciclo se romperá en `i = 4`.

Por lo tanto, la respuesta correcta es **B. 4**, porque es el índice en el que se encuentra el número `1` en la lista y en el momento en que el ciclo `para` se rompe debido a la coincidencia.
