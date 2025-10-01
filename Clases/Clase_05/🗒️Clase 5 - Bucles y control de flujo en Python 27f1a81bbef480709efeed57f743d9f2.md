# 🗒️Clase 5 - Bucles y control de flujo en Python

---

## 1. BUCLES WHILE

### 📖 Concepto

El bucle `while` ejecuta un bloque de código repetidamente mientras una condición sea verdadera. La condición se evalúa antes de cada iteración.

### 📝 Sintaxis

```python
while condicion:
    # código a ejecutar
    # debe haber algo que eventualmente haga la condición False
    # para evitar bucles infinitos
```

### 🔑 Componentes Clave

- **Condición de parada**: expresión booleana que determina si continuar
- **Variable de control**: debe modificarse dentro del bucle
- **Evitar bucles infinitos**: asegurar que la condición eventualmente sea False

---

### ✅ Ejemplos Resueltos

### Ejemplo 1: Contador simple

```python
print("=== Ejemplo 1: Contador del 1 al 5 ===")
contador = 1
while contador <= 5:
    print(f"Número: {contador}")
    contador += 1
print("Fin del bucle\\n")
```

### Ejemplo 2: Suma acumulativa

```python
print("=== Ejemplo 2: Suma de números del 1 al 10 ===")
numero = 1
suma = 0
while numero <= 10:
    suma += numero
    numero += 1
print(f"La suma total es: {suma}\\n")
```

### Ejemplo 3: Validación de entrada

```python
print("=== Ejemplo 3: Validación de contraseña ===")
intentos = 0
max_intentos = 3
password_correcta = "python123"

while intentos < max_intentos:
    password = input(f"Intento {intentos + 1}/{max_intentos} - Ingrese la contraseña: ")
    if password == password_correcta:
        print("¡Acceso concedido!")
        break
    else:
        intentos += 1
        if intentos < max_intentos:
            print("Contraseña incorrecta. Intente nuevamente.\\n")
        else:
            print("Acceso denegado. Ha superado el número de intentos.\\n")
```

---

### 📋 Ejercicios para Practicar

### Ejercicio 1: Cuenta regresiva

**Enunciado**: Crear un programa que imprima una cuenta regresiva desde 10 hasta 1, y al final imprima "¡Despegue!"

**Salida esperada**:

```
10
9
8
...
2
1
¡Despegue!
```

### Ejercicio 2: Tabla de multiplicar

**Enunciado**: Solicitar un número al usuario y mostrar su tabla de multiplicar del 1 al 10 usando while

**Salida esperada (para número 5)**:

```
5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
...
5 x 10 = 50
```

### Ejercicio 3: Suma hasta límite

**Enunciado**: Sumar números consecutivos (1, 2, 3, ...) hasta que la suma supere 100. Mostrar cuántos números se sumaron y la suma final.

**Salida esperada**:

```
Se sumaron 14 números
La suma total es: 105
```

---

### 🎯 Ejercicios Propuestos (No Resolver)

1. **Suma interactiva**: Crear un programa que solicite números al usuario y los sume. El programa debe detenerse cuando el usuario ingrese 0, y mostrar la suma total.
2. **Juego de adivinanza**: Implementar un juego de adivinanza donde el programa piense un número del 1 al 50 y el usuario tenga que adivinarlo. Dar pistas de "mayor" o "menor".
3. **Factorial**: Crear un programa que calcule el factorial de un número ingresado por el usuario usando un bucle while.

---

## 2. BUCLES FOR

### 📖 Concepto

El bucle `for` itera sobre una secuencia (lista, tupla, cadena, range, etc.) ejecutando un bloque de código para cada elemento.

### 📝 Sintaxis

```python
for variable in secuencia:
    # código a ejecutar en cada iteración
    # variable toma el valor de cada elemento
```

### 🔑 Casos de Uso

1. **Iterar sobre listas**: `for elemento in lista`
2. **Iterar sobre cadenas**: `for caracter in cadena`
3. **Iterar con range()**: `for i in range(inicio, fin, paso)`

---

### ✅ Ejemplos Resueltos

### Ejemplo 1: Iterar sobre una lista

```python
print("=== Ejemplo 1: Recorrer una lista de frutas ===")
frutas = ["manzana", "banana", "naranja", "uva", "pera"]
for fruta in frutas:
    print(f"Me gusta la {fruta}")
```

### Ejemplo 2: Iterar sobre una cadena

```python
print("=== Ejemplo 2: Contar vocales en una palabra ===")
palabra = "programacion"
vocales = "aeiouAEIOU"
contador_vocales = 0

for letra in palabra:
    if letra in vocales:
        contador_vocales += 1
        print(f"Vocal encontrada: {letra}")

print(f"Total de vocales: {contador_vocales}")
```

### Ejemplo 3: Usar range() para generar secuencias

```python
print("=== Ejemplo 3: Tabla de cuadrados del 1 al 10 ===")
for numero in range(1, 11):
    cuadrado = numero ** 2
    print(f"{numero}² = {cuadrado}")
```

---

### 📋 Ejercicios para Practicar

### Ejercicio 1: Suma de lista

**Enunciado**: Dada una lista de números, calcular su suma total usando for

**Lista**: `[12, 5, 8, 20, 3, 15]`

**Salida esperada**:

```
La suma total es: 63
```

### Ejercicio 2: Números pares

**Enunciado**: Imprimir todos los números pares del 2 al 20 usando range()

**Salida esperada**:

```
2
4
6
...
18
20
```

### Ejercicio 3: Invertir cadena

**Enunciado**: Recorrer una cadena de texto de atrás hacia adelante e imprimirla

**Cadena**: `"Python"`

**Salida esperada**:

```
n
o
h
t
y
P

```

---

### 🎯 Ejercicios Propuestos (No Resolver)

1. **Contador de nombres largos**: Crear un programa que reciba una lista de nombres y cuente cuántos tienen más de 5 letras.
2. **Conversor de temperaturas**: Dada una lista de temperaturas en Celsius, convertirlas todas a Fahrenheit y mostrar ambos valores. Fórmula: `F = C * 9/5 + 32`
3. **Serie de Fibonacci**: Crear un programa que genere la serie de Fibonacci hasta el término número 15 usando un bucle for.

---

## 3. SENTENCIAS DE CONTROL DE FLUJO

### 📖 Concepto

Las sentencias `break`, `continue` y `pass` permiten controlar el flujo de ejecución dentro de los bucles.

### 📝 Sintaxis y Uso

### 1. BREAK: Termina el bucle inmediatamente

```python
for/while ...:
    if condicion:
        break
```

### 2. CONTINUE: Salta a la siguiente iteración del bucle

```python
for/while ...:
    if condicion:
        continue
```

### 3. PASS: No hace nada, es un marcador de posición

```python
for/while ...:
    if condicion:
        pass
```

---

### ✅ Ejemplos Resueltos

### Ejemplo 1: Break - Buscar un elemento

```python
print("=== Ejemplo 1: Usar break para buscar un número ===")
numeros = [3, 7, 12, 5, 20, 8, 15]
buscar = 20

for num in numeros:
    print(f"Revisando: {num}")
    if num == buscar:
        print(f"¡Número {buscar} encontrado!")
        break
else:
    print(f"Número {buscar} no encontrado")
```

### Ejemplo 2: Continue - Saltar números pares

```python
print("=== Ejemplo 2: Usar continue para saltar pares ===")
for i in range(1, 11):
    if i % 2 == 0:
        continue  # Salta los números pares
    print(f"Número impar: {i}")
```

### Ejemplo 3: Pass - Estructura en desarrollo

```python
print("=== Ejemplo 3: Usar pass como marcador ===")
for letra in "Python":
    if letra in "aeiou":
        pass  # Aquí se implementará lógica futura
    else:
        print(f"Consonante: {letra}")
```

---

### 📋 Ejercicios para Practicar

### Ejercicio 1: Break con validación

**Enunciado**: Solicitar números al usuario hasta que ingrese un número negativo. Mostrar la suma de todos los números positivos ingresados.

**Salida esperada (entrada: 5, 10, 3, -2)**:

```
Suma de números positivos: 18
```

### Ejercicio 2: Continue con filtro

**Enunciado**: Recorrer los números del 1 al 15. Usar continue para saltar los múltiplos de 3 y solo imprimir los demás.

**Salida esperada**:

```
1
2
4
5
7
8
10
11
13
14
```

### Ejercicio 3: Combinación break y continue

**Enunciado**: Recorrer una lista de palabras. Saltar las palabras que empiecen con vocal (continue). Si se encuentra la palabra "fin", terminar el bucle (break).

**Lista**: `["python", "auto", "mesa", "elefante", "fin", "casa"]`

**Salida esperada**:

```
python
mesa
Bucle terminado
```

---

### 🎯 Ejercicios Propuestos (No Resolver)

1. **Menú interactivo**: Crear un menú interactivo que muestre opciones al usuario. Usar continue para opciones inválidas y break para salir del programa.
2. **Validador de contraseña**: Validar una contraseña que debe tener al menos 8 caracteres, un número y una letra mayúscula. Usar continue para saltar caracteres que no cumplan y break cuando se cumplan todos los requisitos.
3. **Sistema de login**: Simular un sistema de login con 3 intentos máximos. Usar break si el login es exitoso, continue si falla pero quedan intentos, y un mensaje final si se agotan los intentos.

---

## 4. CASO DE USO PROPUESTO

### SISTEMA DE GESTIÓN DE CALIFICACIONES

### 📄 Descripción

Crear un programa que permita gestionar las calificaciones de estudiantes. El sistema debe:

### 📋 Funcionalidades del Menú

1. **Ingresar calificaciones de estudiantes**
2. **Mostrar promedio de todas las calificaciones**
3. **Mostrar calificaciones aprobadas (>= 60)**
4. **Buscar calificación de un estudiante específico**
5. **Salir del programa**

### ⚙️ Requisitos Técnicos

- Usar un bucle **while** para mantener el menú activo
- Usar bucles **for** para recorrer listas de calificaciones
- Usar **break** para salir del programa
- Usar **continue** para manejar opciones inválidas
- Validar que las calificaciones estén entre 0 y 100
- Almacenar calificaciones en una lista
- Almacenar nombres de estudiantes en otra lista paralela

### 🌟 Funcionalidades Adicionales

- Mostrar la calificación más alta y más baja
- Contar cuántos estudiantes aprobaron y reprobaron
- Permitir eliminar la última calificación ingresada

### ✅ Validaciones Necesarias

- No permitir calificaciones fuera del rango 0-100
- No permitir buscar estudiantes si no hay datos ingresados
- Manejar entradas de texto cuando se esperan números

### 💡 Ejemplo de Interacción Esperada

```
=== SISTEMA DE GESTIÓN DE CALIFICACIONES ===

1. Ingresar calificaciones
2. Mostrar promedio general
3. Mostrar solo aprobados
4. Buscar estudiante
5. Estadísticas
6. Salir

Opción: 1
¿Cuántos estudiantes desea ingresar? 3

Estudiante 1:
Nombre: Juan
Calificación: 85

Estudiante 2:
Nombre: María
Calificación: 92

Estudiante 3:
Nombre: Pedro
Calificación: 58

Calificaciones ingresadas exitosamente.

[El menú se vuelve a mostrar...]

Opción: 2
Promedio general: 78.33

[Continúa el ciclo del menú hasta que el usuario elija salir]
```