# Documentación de ejercicios (Tema 2)

Este documento resume los ejercicios del cuaderno `py_ejercicios/tema2.ipynb`. Cada sección describe el objetivo del ejercicio, los pasos principales y el resultado esperado.

## 1. Tipos de datos básicos

- **Objetivo:** practicar la creación de variables `int`, `float`, `bool` y `str`.
- **Descripción:** se definen las variables `age`, `height`, `is_student` y `name`, y se imprimen sus valores.
- **Salida esperada:** los valores `25`, `1.75`, `True` y `Ana` en líneas separadas.

## 2. Operaciones con listas

- **Objetivo:** reforzar métodos fundamentales de listas (`append`, `insert`, `remove`) y cálculos simples.
- **Pasos principales:**
  - Lista inicial `numeros = [10, 20, 30, 40, 50]`.
  - Añadir `60`, insertar `15` en la posición 1 y eliminar `30`.
  - Calcular la suma y el promedio de los valores finales.
- **Salida esperada:** lista `[10, 15, 20, 40, 50, 60]`, suma `195` y promedio `32.5`.

## 3. Trabajo con tuplas

- **Objetivo:** practicar la creación de tuplas, desempaquetado y concatenación.
- **Descripción:** se crea `contacto = ("Ana García", "ana@ejemplo.com", "555-1234")`, se desempaqueta en variables y se construye `contacto_completo` añadiendo `"Madrid"`.
- **Salida esperada:** impresión del nombre, correo, teléfono y la tupla extendida.

## 4. Diccionarios anidados

- **Objetivo:** manipular un diccionario de diccionarios y actualizar información.
- **Pasos principales:**
  - Se definen contactos iniciales con datos personales.
  - Se consulta el correo de `persona2`, se agrega `persona4` y se actualiza el teléfono de `persona1`.
  - Se recorre el diccionario para listar los nombres almacenados.
- **Salida esperada:** el diccionario actualizado, el correo de David, el nuevo número de Ana y la lista de nombres.

## 5. Operaciones con conjuntos

- **Objetivo:** utilizar operaciones de conjuntos (`intersection`, `difference`, `union`) a partir de dos listas.
- **Descripción:** con `lista1` y `lista2` se calculan elementos comunes, exclusivos y la unión.
- **Salida esperada:** `{4, 5, 6}`, `{1, 2, 3}`, `{8, 9, 7}` y `{1, 2, 3, 4, 5, 6, 7, 8, 9}` respectivamente.

## 6. `defaultdict` aplicado a taxonomías

- **Objetivo:** mostrar cómo `defaultdict` simplifica estructuras anidadas.
- **Descripción:** se construye una jerarquía `taxonomia` con categorías de animales y plantas, rellenando listas sin comprobar si existen previamente.
- **Salida esperada:** lista `['perro', 'gato']` para mamíferos y lista vacía para `plantas["flores"]`, junto con la estructura completa del `defaultdict`.

## 7. Comparativa de conteo

- **Objetivo:** comparar el rendimiento de tres enfoques para contar elementos repetidos.
- **Metodología:**
  - Se genera una lista con 1 000 000 de `"a"`, 500 000 de `"b"` y 250 000 de `"c"`.
  - Se mide el tiempo usando (1) diccionario estándar, (2) `defaultdict(int)` y (3) `Counter`.
- **Conclusión:** `Counter` es el más rápido en este escenario, seguido de `defaultdict`; el diccionario manual resulta más lento.
