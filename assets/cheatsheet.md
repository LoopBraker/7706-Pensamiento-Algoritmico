# Cheat Sheet de Funciones Básicas de Python

## 1. Funciones de Manejo de Cadenas

- **`len()`**: Devuelve la longitud de una cadena.
  ```python
  cadena = "Hola"
  print(len(cadena))  # Salida: 4
  ```

- **`str()`**: Convierte un valor a una cadena.
  ```python
  numero = 123
  print(str(numero))  # Salida: '123'
  ```

- **`upper()`**: Convierte una cadena a mayúsculas.
  ```python
  cadena = "hola"
  print(cadena.upper())  # Salida: 'HOLA'
  ```

- **`lower()`**: Convierte una cadena a minúsculas.
  ```python
  cadena = "HOLA"
  print(cadena.lower())  # Salida: 'hola'
  ```

- **`split()`**: Divide una cadena en una lista usando un separador.
  ```python
  cadena = "Hola mundo"
  print(cadena.split())  # Salida: ['Hola', 'mundo']
  ```

## 2. Funciones de Manejo de Listas

- **`append()`**: Añade un elemento al final de la lista.
  ```python
  lista = [1, 2, 3]
  lista.append(4)
  print(lista)  # Salida: [1, 2, 3, 4]
  ```

- **`remove()`**: Elimina el primer elemento con el valor especificado.
  ```python
  lista = [1, 2, 3, 2]
  lista.remove(2)
  print(lista)  # Salida: [1, 3, 2]
  ```

- **`pop()`**: Elimina y devuelve el último elemento de la lista.
  ```python
  lista = [1, 2, 3]
  print(lista.pop())  # Salida: 3
  print(lista)  # Salida: [1, 2]
  ```

- **`sort()`**: Ordena la lista en orden ascendente.
  ```python
  lista = [3, 1, 2]
  lista.sort()
  print(lista)  # Salida: [1, 2, 3]
  ```

- **`reverse()`**: Invierte el orden de los elementos en la lista.
  ```python
  lista = [1, 2, 3]
  lista.reverse()
  print(lista)  # Salida: [3, 2, 1]
  ```

## 3. Funciones de Control de Flujo

-  **Iterar en una lista:**
  ```python
  lista = [1,2,3,4,5]
  for i in lista:
      print(i)  # Salida: 1 2 3 4 5
   ```
   
- **`range()`**: Genera una secuencia de números.
  ```python
  for i in range(5):
      print(i)  # Salida: 0 1 2 3 4
  ```

- **`enumerate()`**: Devuelve pares índice-valor para una lista.
  ```python
  lista = ['a', 'b', 'c']
  for indice, valor in enumerate(lista):
      print(indice, valor)  # Salida: 0 a, 1 b, 2 c
  ```

## 4. Funciones de Entrada y Salida

- **`input()`**: Captura la entrada del usuario.
  ```python
  nombre = input("¿Cuál es tu nombre?")
  edad = int(input("Ingresa tu edad: "))
  print("Hola, " + nombre)
  print("naciste en ", 2024 - edad)
  ```

- **`print()`**: Imprime un mensaje en la consola.
  ```python
  print("Hola, mundo!")  # Salida: Hola, mundo!
  ```

- **`print()` con `format`**: Imprime un mensaje que incluye una variable formateada.
  ```python
  nombre = "Carlos"
  edad = 22
  print("Hola, mi nombre es {} y tengo {} años.".format(nombre, edad))
  # Salida: Hola, mi nombre es Carlos y tengo 22 años.
  ```

- **`print()` con coma**: Imprime múltiples parámetros separando texto y variables con comas.
```python
nombre = "Carlos" 
edad = 22 
print("Hola, mi nombre es", nombre, "y tengo", edad, "años.") # Salida: Hola, mi nombre es Carlos y tengo 22 años.
```
  
## 5. Funciones Matemáticas

- **`abs()`**: Devuelve el valor absoluto de un número.
  ```python
  print(abs(-5))  # Salida: 5
  ```

- **`round()`**: Redondea un número al número especificado de dígitos.
  ```python
  print(round(3.14159, 2))  # Salida: 3.14
  ```

- **`sum()`**: Devuelve la suma de una lista de números.
  ```python
  numeros = [1, 2, 3, 4]
  print(sum(numeros))  # Salida: 10
  ```

- **`%`**: Devuelve el residuo de la división entre dos números. Puedes usar la operación módulo para verificar si un número es par o impar. Un número es par si el residuo de su división por 2 es 0, y es impar si el residuo es 1. Otra aplicación de La operación módulo es una forma rápida de verificar si un número es divisible por otro. 
  ```python
  resultado = 10 % 5
  print(resultado)  # Salida: 0
  ```

## 6. Ciclos y condicionales

- **Estructura básica del `if`**:
  ```python
  edad = 18
  if edad >= 18:
      print("Eres mayor de edad.")
  else:
      print("Eres menor de edad.")
  ```

- **Uso de `elif`**:
  ```python
  nota = 85
  if nota >= 90:
      print("Excelente")
  elif nota >= 80:
      print("Muy bien")
  elif nota >= 70:
      print("Bien")
  else:
      print("Necesitas mejorar")
  ```

- **Estructura básica del `while`**:
  ```python
  contador = 0
  while contador < 5:
      print("El contador es:", contador)
      contador += 1
  ```

- **Uso de `while` con `break`**:
  ```python
  contador = 0
  while True:
      print("El contador es:", contador)
      contador += 1
      if contador >= 5:
          break
  ```

- **Uso de `while` con `continue`**:
  ```python
  contador = 0
  while contador < 5:
      contador += 1
      if contador == 3:
          continue
      print("El contador es:", contador)
  # Salida: 1, 2, 4, 5 (el 3 se salta por el continue)
  ```

## 7. Funciones básicas arreglos bidimensionales

- **Importar NumPy**: Antes de usar cualquier función de NumPy, necesitas importar el módulo.
   ```python
   import numpy as np
   ```

 - **Crear un Arreglo Bidimensional desde una Lista de Listas**:
   ```python
   lista = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
   arreglo = np.array(lista)
   print(arreglo)
   # Salida:
   # [[1 2 3]
   #  [4 5 6]
   #  [7 8 9]]
   ```

- **Crear un Arreglo Bidimensional con Ceros**:
   ```python
   arreglo_ceros = np.zeros((3, 3))
   print(arreglo_ceros)
   # Salida:
   # [[0. 0. 0.]
   #  [0. 0. 0.]
   #  [0. 0. 0.]]
   ```

 - **Acceder a un Elemento Específico en un Arreglo Bidimensional**:
   ```python
   elemento = arreglo[1, 2]  # Accede al elemento en la fila 2, columna 3
   print(elemento)
   # Salida: 6
   ```

- **Acceder a una Fila Completa**:
   ```python
   fila = arreglo[1, :]
   print(fila)
   # Salida: [4 5 6]
   ```

- **Acceder a una Columna Completa**:
   ```python
   columna = arreglo[:, 1]
   print(columna)
   # Salida: [2 5 8]
   ```

-  **Sumar Todos los Elementos de un Arreglo Bidimensional**:
    ```python
    suma = np.sum(arreglo)
    print(suma)
    # Salida: 45
    ```

- **Calcular el Promedio de los Elementos de un Arreglo Bidimensional**:
    ```python
    promedio = np.mean(arreglo)
    print(promedio)
    # Salida: 5.0
    ```


