# Programación Modular en Python: divide y venceras

La programación modular es una estrategia clave para lidiar con la complejidad del código, especialmente en proyectos grandes. La idea es simple: dividir el código en módulos independientes que resuelvan tareas específicas. En Python, esto se logra creando funciones y organizando el código en bloques lógicos.

### ¿Por Qué Modularizar? 
Un beneficio esencial de la modularidad es la facilidad de mantenimiento y reutilización. Por ejemplo, imagina que tienes una función que calcula el precio total de un producto, impuestos incluidos. Si modularizas esta función, podrás reutilizarla cada vez que necesites ese cálculo en tu programa sin tener que escribir el código desde cero. 

Aquí tienes un ejemplo básico en Python:

```python
def calcular_precio_total(precio, impuesto):
    """Calcula el precio total incluyendo impuestos"""
    total = precio + (precio * impuesto)
    return total
```

Una vez que tienes esta función, puedes reutilizarla en cualquier parte de tu programa para calcular precios, sin preocuparte por recalcular el impuesto en cada línea de código. Así es como el código modular facilita la reutilización.

### Variables Locales: Manteniendo el Orden

Dentro de cada módulo o función, es común trabajar con variables locales, es decir, variables que existen solo en el ámbito de esa función. Esto asegura que cada función tenga un “espacio de trabajo” aislado. Por ejemplo:

```python
def calcular_descuento(precio, porcentaje):
    """Calcula el descuento a aplicar a un precio"""
    descuento = precio * (porcentaje / 100)  # Variable local
    precio_final = precio - descuento
    return precio_final
```

Aquí, `descuento` y `precio_final` son variables locales de la función `calcular_descuento`. Estas variables no existen fuera de la función, por lo que otros módulos o funciones no pueden acceder a ellas, evitando conflictos y errores inesperados.

### Independencia de los Módulos: ¿Siempre Total?

Aunque la independencia de los módulos es ideal, en ocasiones es necesario que los módulos compartan cierta información. En estos casos, una práctica común es pasar variables como argumentos a las funciones, en lugar de depender de variables globales. Las variables globales pueden hacer que el código sea difícil de entender y propenso a errores.

Veamos un ejemplo de cómo podrías manejar la independencia de módulos y aún compartir datos importantes:

```python
def calcular_precio_con_descuento(precio, impuesto, descuento):
    """Calcula el precio total aplicando un descuento y el impuesto"""
    precio_descuento = calcular_descuento(precio, descuento)  # Reutilizamos la función calcular_descuento
    total = calcular_precio_total(precio_descuento, impuesto)  # Reutilizamos la función calcular_precio_total
    return total
```

Aquí, `calcular_precio_con_descuento` reutiliza las funciones `calcular_descuento` y `calcular_precio_total`. Este enfoque modular permite que cada función haga su trabajo específico, mientras `calcular_precio_con_descuento` se encarga de coordinar el flujo de datos entre ellas.

### Buenas Prácticas en Programación Modular

1. **Mantén los módulos específicos**: Cada función debe hacer solo una cosa y hacerla bien.
2. **Usa variables locales**: Esto evita que datos se mezclen accidentalmente entre módulos.
3. **Comunicación clara entre funciones**: Usa parámetros para pasar información, en lugar de depender de variables globales.
4. **Reutiliza funciones**: Modularizar permite llamar a funciones en diferentes partes del programa sin duplicar código.
