# 🧗🏽Práctica 2

> Entregar todos los ejercicios propuestos de esta clase en un archivo con nombre practica_02.ipynb.
> 
1. Asigna un valor entero 2001 a la variable `space_odyssey` y muestra su valor.
2. Descubre el tipo del literal 'Good night & Good luck'.
3. Identifica el tipo del literal True.
4. Asigna la expresión 10 * 3.0 a la variable `result` y muestra su tipo.

## 📝 5. Ejercicios resueltos:

> Ejecutar los siguientes códigos. Modifícalos cambiando los datos  nombres de las varaibles
> 

### Ejercicio 1: Crear variables

```python
nombre = "Carlos"
edad = 22
altura = 1.80
es_estudiante = True

print(nombre, edad, altura, es_estudiante)

```

---

### Ejercicio 2: Identificar tipos

```python
x = 10
y = 3.5
z = "Python"
a = False

print(type(x))  # int
print(type(y))  # float
print(type(z))  # str
print(type(a))  # bool

```

---

### Ejercicio 3: Operaciones básicas

```python
a = 10
b = 3

print(a + b)  # suma
print(a - b)  # resta
print(a * b)  # multiplicación
print(a / b)  # división

```

---

### Ejercicio 4: Conversión de datos

```python
edad = "25"
edad_num = int(edad)
print(edad_num + 5)  # 30

```

---

### 🤔 Ejercicio 5

1. Crea una variable con tu **nombre**, otra con tu **edad**, otra con tu **altura**, y un booleano que indique si eres estudiante.
2. Usa `print()` para mostrar una presentación como:
    
    ```
    Hola, me llamo Ana, tengo 22 años, mido 1.65 y es True que soy estudiante.
    ```
    
3. Calcular el área de un círculo con radio 7. **Salida esperada:** `Área: 153.938...`
4. Convertir un número decimal `7.8` a entero. **Salida esperada:** `7`

### 🤔 Ejercicio 6

Crea un programa en Python que simule una tabla básica de 3 filas y 2 columnas (por ejemplo, Nombre y Edad) usando \t para separar las columnas y \n para separar las filas. Asegúrate de incluir encabezados.

Ejemplo de Salida:

```python
Nombre    Edad
Jose      25
Marta     30
Peter     28
```

### 🤔Ejercicio 7: Concatenación

Escribe un programa en Python que concatene una lista de tres ciudades (por ejemplo, "Madrid", "Barcelona", "Valencia") en una sola cadena, separadas por comas y un espacio, y luego añada un mensaje inicial como "Ciudades visitadas: " usando el operador `+`.

Salida esperada:

```python
Ciudades visitadas: Madrid, Barcelona, Valencia
```

### 🤔Ejercicio 8: Interpolación

Desarrolla un programa en Python que use interpolación con `.format()` para crear una tabla simple de estudiantes. Incluye nombre, edad y ciudad para al menos dos estudiantes en la frase "Estudiante: {nombre}, edad: {edad}, ciudad: {ciudad}".

Salida esperada:

```python
Estudiante: Ana, edad: 22, ciudad: Sevilla
Estudiante: Luis, edad: 25, ciudad: Bilbao
```

### 🤔Ejercicio 9: Count, Len y Upper

Crea un programa en Python que tome una frase, cuente las ocurrencias de la letra "e" con `.count("e")`, obtenga su longitud con `len()`, conviértala a mayúsculas con `.upper()`, y luego imprima un mensaje que indique cuántas "e" hay y la longitud de la frase original.

Salida esperada:

```python
La frase original tiene 47 letras.
La letra 'e' aparece 6 veces.
Frase en mayúsculas: HOLA, ESTE ES UN EJEMPLO DE FRASE CON VARIAS EES.
```

### 🤔Ejercicio 10: **Conversor de temperaturas**

Escribe un programa que pida al usuario una temperatura en grados Celsius (como número decimal) y la convierta a Fahrenheit usando la fórmula: `F = C * 9/5 + 32`
Muestra el resultado con un mensaje claro.

### 🤔Ejercicio 11: **Área de un rectángulo**

Escribe un programa que pida al usuario la longitud y el ancho de un rectángulo (como números decimales) y calcule el área (área = longitud * ancho). Muestra el resultado con un mensaje.

### 🤔Ejercicio 12: Sistema de Calificaciones

Crea un programa que:

- Solicite el nombre del estudiante
- Solicite 3 calificaciones (pueden ser decimales)
- Calcule el promedio
- Determine la letra de calificación según:
    - A: 90-100
    - B: 80-89
    - C: 70-79
    - D: 60-69
    - F: menos de 60
- Muestre un reporte completo

Salida esperada:

```python
Estudiante: María García
Calificaciones: 85, 92, 78
Promedio: 85.0
Calificación: B
```

### 🤔Ejercicio 13: Analizador de Entradas Múltiples

Crea un programa que solicite **5 entradas diferentes** al usuario y genere un reporte completo sobre el análisis booleano de cada una, incluyendo estadísticas generales.

### Instrucciones:

1. Solicita **5 datos diferentes** al usuario:
    - Un nombre de usuario
    - Una contraseña (puede estar vacía)
    - Un número favorito
    - Una palabra secreta (puede estar vacía)
    - Un código numérico
2. Para cada entrada:
    - Convierte a `bool()`
    - Calcula la longitud del texto original
    - Si es un número, muestra también su valor numérico y conversión booleana
3. Genera estadísticas:
    - Cuántas entradas fueron `True`
    - Cuántas entradas fueron `False`
    - Total de caracteres ingresados
    - Promedio de longitud por entrada

Salida esperada (ejemplo):

```
 ANALIZADOR DE ENTRADAS MÚLTIPLES
Ingresa 5 datos diferentes para analizar:

1. Nombre de usuario: admin
2. Contraseña (puede estar vacía): 
3. Tu número favorito: 7
4. Palabra secreta (puede estar vacía): python
5. Código numérico: 0

==================================================
REPORTE DE ANÁLISIS
==================================================
1. Usuario: 'admin' → Longitud: 5 → bool(): True
2. Contraseña: '' → Longitud: 0 → bool(): False
3. Número favorito: '7' → Valor: 7 → bool(): True
4. Palabra secreta: 'python' → Longitud: 6 → bool(): True
5. Código: '0' → Valor: 0 → bool(): False

==================================================
ESTADÍSTICAS GENERALES
==================================================
Entradas que son True: 3
Entradas que son False: 2
Total de caracteres ingresados: 12
Promedio de longitud por entrada: 2.4

Porcentaje de entradas con contenido: 60.0%
Números ingresados - Favorito: 7, Código: 0
Suma total de ambos números: 7
```