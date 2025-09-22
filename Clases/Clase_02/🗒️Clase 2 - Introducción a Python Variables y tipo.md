# 🗒️Clase 2 - Introducción a Python: Variables y tipos de datos

# Repaso

---

### ¿Por qué Python?

Python es como el "cuchillo suizo" de los lenguajes de programación:

- **Sintaxis clara**: Se lee casi como inglés
- **Versatilidad**: Desde aplicaciones web hasta inteligencia artificial
- **Comunidad activa**: Millones de desarrolladores en todo el mundo
- **Demanda laboral**: Uno de los lenguajes más solicitados

### 🔧 Desarrollo Teórico

---

### ¿Qué es Python?

Python es un **lenguaje de programación interpretado**, lo que significa:

- No necesitas compilar el código antes de ejecutarlo
- Puedes probar código línea por línea
- Es perfecto para aprender y experimentar

**Analogía**: Imagina que Python es como tener una conversación directa con la computadora, mientras que otros lenguajes requieren que escribas una carta completa antes de enviarla.

## 💻 Práctica Guiada

### Actividad 1: Verificación de Instalación

### Verificar Python

Abre la terminal/línea de comandos y ejecuta (En visual Studio Code) :

```python
python --version
python3 --version
```

**Salida esperada:**

```
	Python 3.12.x
```

### Primera interacción con el intérprete

Escribe `python` (o python3) en la terminal:

```python
>>> print("¡Python está funcionando!")
>>> 2 + 3
>>> "Hola" + " " + "Mundo"
>>> exit()

```

### Actividad 2: Configuración de VS Code

### Paso 1: Crear tu primer archivo Python

1. Abre VS Code
2. Crea una nueva carpeta llamada `python_curso`
3. Dentro de la carpeta, crea un archivo `primer_programa.py`

### Paso 2: Escribir el código

```python
# Mi primer programa en Python
print("¡Hola, mundo!")
print("Mi nombre es [TU_NOMBRE]")
print("¡Estoy aprendiendo Python!")

```

### Paso 3: Ejecutar el programa

- **Opción 1**: Botón "Run" (triángulo) en VS Code
- **Opción 2**: Terminal: `python primer_programa.py`
- **Opción 3**: F5 para debug mode - Lo veremos después

### Actividad 3: Explorando el Intérprete Interactivo

### Calculadora Básica

```python
>>> 15 + 25
40
>>> 100 / 4
25.0
>>> 2 ** 3  # Potenciación
8
>>> 17 % 5  # Módulo (resto)
2

```

### Trabajando con Texto

```python
>>> nombre = "Python"
>>> print("Me gusta", nombre)
Me gusta Python
>>> print(nombre * 3)
PythonPythonPython
>>> len(nombre)  # Longitud del texto
6
```

### Actividad 4: Comentarios y Documentación

### Tipos de Comentarios

```python
# Esto es un comentario de una línea

"""
Esto es un comentario
de múltiples líneas
o docstring
"""

# Comentarios para explicar código complejo
edad = 25  # Edad del usuario en años
saludo = "¡Hola!"  # Mensaje de bienvenida

# Comentarios para dividir secciones
# ===== CÁLCULOS MATEMÁTICOS =====
resultado = (10 + 5) * 2

# ===== MOSTRAR RESULTADOS =====
print(f"El resultado es: {resultado}")

```

### Buenas Prácticas de Comentarios

```python
# ❌ Comentario innecesario
x = x + 1  # Incrementa x en 1

# ✅ Comentario útil
x = x + 1  # Contador de intentos de login

# ✅ Explicando lógica compleja
# Calculamos el descuento basado en la edad del cliente
# Menores de 18: 50% descuento
# Mayores de 65: 30% descuento
# Resto: sin descuento
if edad < 18:
    descuento = 0.5
elif edad > 65:
    descuento = 0.3
else:
    descuento = 0.0

```

---

## 🎯 Ejercicios Básicos

### Ejercicio 1: Mi Presentación

**Enunciado**: Crea un programa que imprima tu presentación personal incluyendo nombre, edad y ciudad.

**Solución**:

```python
# Mi presentación personal
print("=== MI PRESENTACIÓN ===")
print("Nombre: Juan Pérez")
print("Edad: 25 años")
print("Ciudad: Madrid")
print("Pasatiempo: Aprender Python")
print("========================")

```

### Ejercicio 2: Calculadora Simple

**Enunciado**: Usa el **intérprete interactivo desde VSCode** para resolver: (15 + 25) * 3 - 10

**Solución**:

```python
# En el intérprete interactivo
>>> (15 + 25) * 3 - 10
110

# En un script
resultado = (15 + 25) * 3 - 10
print(f"El resultado de (15 + 25) * 3 - 10 = {resultado}")

```

<aside>

En Google Colab

Descargar archivo [my_script.py](https://tajamar365.sharepoint.com/:u:/s/356033.2PYTHONF241783AA/EQ1jUanYTt5HmScCEmc131sBVyrq1-u2XS4eaXfs4qSbRg?e=cnqarn)

Si tienes un archivo llamado **my_script.py**, puedes ejecutarlo en una celda de código en google colab así: `%run my_script.py` o `!python my_script.py`

También puedes ejecutarlo directamente desde la terminal integrada de colab usando: `python my_script.py`

</aside>

Vamos al notebook de google colab…

### Ejercicio 3: Mensajes Personalizados

**Enunciado**: Crea un programa que muestre 3 mensajes diferentes usando print().

**Solución**:

```python
# Mensajes personalizados
print("🌟 ¡Bienvenido al curso de Python!")
print("📚 Cada día aprenderás algo nuevo")
print("🚀 ¡El límite es tu imaginación!")

```

### Ejercicio 4: Comentarios Descriptivos

**Enunciado**: Toma el código de la calculadora y añade comentarios explicativos.

**Solución**:

```python
# Programa: Calculadora básica
# Autor: Estudiante de Python
# Fecha: [Fecha actual]

# Definimos los números a operar
numero1 = 15
numero2 = 25
numero3 = 3
descuento = 10

# Realizamos el cálculo principal
# Primero sumamos los dos primeros números
suma = numero1 + numero2

# Multiplicamos el resultado por el tercer número
multiplicacion = suma * numero3

# Finalmente restamos el descuento
resultado_final = multiplicacion - descuento

# Mostramos el resultado al usuario
print(f"Resultado: {resultado_final}")

```

---

---

---

<aside>

## 🚀 Practica 1. Ejercicios Intermedios

> Entregar en uno o varios ficheros .py o todo en un notebook en formato .ipynb (Colab o Visual Studio).
El archivo debe entregarse con nombre practica_01.ipynb o .py
> 

## 🚀Parte 1

### Ejercicio 1: Información del Sistema

**Enunciado**: Crea un script que muestre información sobre tu instalación de Python usando comentarios explicativos.

**Solución**:

```python
# Programa de información del sistema Python
# Este programa muestra detalles de la instalación

# Importamos el módulo sys para obtener información del sistema
import sys

# Mostramos la versión de Python
print("=== INFORMACIÓN DEL SISTEMA ===")
print(f"Versión de Python: {sys.version}")
print(f"Plataforma: {sys.platform}")

# Información adicional
print("\n=== DETALLES ADICIONALES ===")
print(f"Ruta del ejecutable: {sys.executable}")
print(f"Codificación por defecto: {sys.getdefaultencoding()}")

```

### Ejercicio 2: Calculadora de Propinas

**Enunciado**: Crea un programa que calcule propinas del 10%, 15% y 20% para una cuenta de $50.

**Solución**:

```python
# Calculadora de propinas para restaurante
# Calcula diferentes porcentajes de propina

# Configuración inicial
cuenta_total = 50.0  # Total de la cuenta en dólares

# Cálculo de propinas comunes
propina_10 = cuenta_total * 0.10  # 10% de propina
propina_15 = cuenta_total * 0.15  # 15% de propina (estándar)
propina_20 = cuenta_total * 0.20  # 20% de propina (buen servicio)

# Mostramos los resultados
print("=== CALCULADORA DE PROPINAS ===")
print(f"Cuenta total: ${cuenta_total:.2f}")
print(f"Propina 10%: ${propina_10:.2f} (Total: ${cuenta_total + propina_10:.2f})")
print(f"Propina 15%: ${propina_15:.2f} (Total: ${cuenta_total + propina_15:.2f})")
print(f"Propina 20%: ${propina_20:.2f} (Total: ${cuenta_total + propina_20:.2f})")

```

### Ejercicio 3: Generador de Mensajes

**Enunciado**: Crea diferentes variaciones del mensaje "Hola mundo" usando operaciones con strings.

**Solución**:

```python
# Generador de variaciones de "Hola Mundo"
# Demuestra diferentes formas de manipular strings

# Mensaje básico
mensaje_base = "Hola"
destinatario = "Mundo"

# Diferentes formas de mostrar el saludo
print("=== VARIACIONES DE SALUDO ===")
print(mensaje_base + " " + destinatario)  # Concatenación básica
print(f"{mensaje_base} {destinatario}!")  # F-string (recomendado)
print(mensaje_base, destinatario)  # Usando print con múltiples argumentos

# Variaciones creativas
print("\n=== VERSIONES CREATIVAS ===")
print(mensaje_base.upper() + " " + destinatario.lower())  # HOLA mundo
print((mensaje_base + " " + destinatario + "! ") * 3)  # Repetición
print(f"{'*' * 20}")  # Línea decorativa
print(f"*{mensaje_base:^18}*")  # Centrado con decoración
print(f"*{destinatario:^18}*")
print(f"{'*' * 20}")

```

### Ejercicio 4: Script de Bienvenida

**Enunciado**: Crea un script que simule la bienvenida a una aplicación con información detallada.

**Solución**:

```python
# Script de bienvenida a la aplicación
# Simula la pantalla inicial de un programa

# Información de la aplicación
nombre_app = "Python Learning Center"
version = "1.0.0"
autor = "Estudiante Python"

# Creamos una línea decorativa
linea_decorativa = "=" * 50

# Pantalla de bienvenida
print(linea_decorativa)
print(f"    🐍 {nombre_app.upper()} 🐍")
print(linea_decorativa)
print(f"Versión: {version}")
print(f"Desarrollado por: {autor}")
print(f"Lenguaje: Python {3.11}")  # Versión de Python
print()

# Mensaje de bienvenida personalizado
print("🌟 ¡Bienvenido a tu journey de aprendizaje! 🌟")
print()

# Instrucciones iniciales
print("📋 INSTRUCCIONES:")
print("   • Sigue las lecciones paso a paso")
print("   • Practica con los ejercicios")
print("   • No temas experimentar")
print("   • ¡Diviértete aprendiendo!")
print()

print(linea_decorativa)
print("         ¡Presiona ENTER para continuar!")
print(linea_decorativa)

```

---

## 🚀Parte 2

## 🎪 Ejercicios Propuestos

### Ejercicio 1: Generador de Arte ASCII

**Enunciado**: Crea un programa que genere un dibujo simple usando caracteres ASCII y comentarios explicativos.

**Salida Esperada**:

```
=== GENERADOR DE ARTE ASCII ===

      🌟 MI PRIMERA CASA EN PYTHON 🌟

        🏠 Casa Simple 🏠

           /\
          /  \
         /____\
        |  🚪  |
        |   ⬜ |
        |______|

    Creado con: Python 3.11
    Caracteres usados: 45
    Líneas de código: 12

=== ¡Arte ASCII completado! ===

```

### Ejercicio 2 Generador de Patrones

**Enunciado**: Crea un programa que genere 3 patrones diferentes usando repetición de caracteres y print().

**Salida Esperada**:

```
=== GENERADOR DE PATRONES ===

🔸 Patrón 1: Escalera Ascendente
*
**
***
****
*****

🔸 Patrón 2: Pirámide Centrada
    *
   ***
  *****
 *******
*********

🔸 Patrón 3: Marco Decorativo
**********
*        *
*  HOLA  *
*        *
**********

¡Patrones generados exitosamente!

```

---

## 🚀Parte 3

**Instrucciones**: Elige uno de estos ejercicios para realizar de forma independiente:

1. **Personalizador**: Modifica el "Hola Mundo" para mostrar tu información personal (información falsa)
2. **Calculadora Personal**: Calcula cuántos días has vivido

</aside>

---

---

---

# **Clase 2: Variables y Tipos de Datos**

---

## Introducción a variables

> Podemos entender las variables como contenedores que pueden almacenar valores. Éstos valores que hay dentro del contenedor pueden variar, por ello su nombre "variable". Una variable se compone de:
> 
- Un nombre.
- Un valor.

Dentro de las convenciones de Python, se estipula que el nombre de una variable comienza con minúscula, y si se requiere utilizar más de una palabra, éstas deben estar unidas por un guión bajo o underscore. Los nombres de las variables no pueden tener espacios. Es importante también utilizar nombres que sean representativos del valor que se quiere almacenar. Por ejemplo, si queremos crear una variable de que almacene la cantidad de alumnos de un curso, su nombre podría ser `cant_alumnos_algebra`.

Además, una variable poseerá un tipo de dato asociado, según el valor que se le asigne. Los tipos de datos pueden ser, entre otros, integer, string, double o bool.

En Python se usa el símbolo `=` para asignar un valor a una variable:

![image.png](image.png)

👉 En Python, no necesitamos declarar el tipo de la variable, el intérprete lo detecta automáticamente.

## Algunos ejemplos de asignaciones a variables:

```python
total_population = 157503
avg_temperature = 16.8
city_name = 'San Cristóbal de La Laguna'

```

<aside>

**Nota:** Hay que diferenciar la asignación en Python con la igualación en matemáticas. El símbolo `=` lo hemos aprendido desde siempre como una equivalencia entre dos expresiones algebraicas, sin embargo en Python nos indica una sentencia de asignación, del valor (en la derecha) al nombre (en la izquierda).

</aside>

En Python asignamos valores a las variables siguiendo el siguiente formato: `nombre_variable = valor`

```python
x = 1
x
```

*Salida:*

1

```python
y = "hola"
y
```

*Salida:*

'hola'

<aside>

### Restricciones sobre los nombres de las variables

- No pueden empezar ni contener caracteres especiales
- No pueden empezar por números
- No pueden ser llamadas igual que las palabras claves reservadas en Python
- No pueden contener espacios
</aside>

> **Observación.** Conviene que al darle nombre a una variable, éste tenga sentido en cuanto al dato que guarde, para que así resulte mucho más fácil la comprensión por parte de quien lea el código.
> 

 A día de hoy, si los nombres de las variables están compuestos por múltiples palabras, hay 4 formas de escribir dichos nombres:

- `camelCase`: nombreMascota
- `PascalCase`: NombreMascota
- `snake_case`: nombre_mascota
- `kebab-case`: nombre-mascota

> **Importante:** Los nombres de variables son *case-sensitive*. Por ejemplo, `stuff` y `Stuff` son nombres diferentes.
> 

<aside>

### Como regla general:

- Usar nombres para variables (ejemplo `article`).
- Usar verbos para funciones (ejemplo `get_article()`).
- Usar adjetivos para booleanos (ejemplo `available`).
</aside>

## Palabras clave en Python

Las palabras clave en Python son las que se muestran con el siguiente chunk de código.

```python
import keyword
keyword.kwlist
```

Output:

- ['False', 'None', 'True', 'and', 'as', 'assert', 'break', 'class', 'continue', 'def', 'del', 'elif', 'else', 'except', 'finally', 'for', 'from', 'global', 'if', 'import', 'in', 'is', 'lambda', 'nonlocal', 'not', 'or', 'pass', 'raise', 'return', 'try', 'while', 'with', 'yield']

## Asignando un valor a una variable

### Integers

En Python -y en muchos otros lenguajes de programación- los números enteros se denominan *enteros* y *Integers*. De tal manera, podemos decir que: La variable `entero` contiene un Integer y su valor es 27.

```
entero = 27

```

Como el valor de la variable puede cambiar, a la variable `entero` se le puede asignar un nuevo número sin problemas.

```
entero = 33

```

---

# Declarando múltiples variables en una sola línea

Se hace del siguiente modo:

```python
age, name = 22, "María"
```

```python
age
```

Output: 22

```python
name
```

Output: "María"

---

### Python nos ofrece la posibilidad de hacer una asignación múltiple de la siguiente manera:

```
tres = three = drei = 3
```

En este caso las tres variables utilizadas en el *lado izquierdo* tomarán el valor 3.

---

### Asignando una variable a otra variable

Las asignaciones que hemos hecho hasta ahora han sido de un valor literal a una variable. Pero nada impide que podamos hacer asignaciones de una variable a otra variable:

```
people = 157503
total_population = people
total_population
```

157503

---

### Conocer el valor de una variable

Hemos visto previamente cómo asignar un valor a una variable, pero aún no sabemos cómo *comprobar* el valor que tiene dicha variable. Para ello podemos utilizar dos estrategias:

1. Si estamos en un intérprete (*shell* o consola) de Python, basta con que usemos el nombre de la variable:

```
final_stock = 38934
final_stock
```

38934

1. Si estamos escribiendo un programa desde el editor, debemos hacer uso de print():

```
final_stock = 38934
print(final_stock)
```

> Nota: **print()** sirve también cuando estamos en una sesión interactiva de Python (*shell*).
> 

### Conocer el tipo de una variable

Para poder descubrir el tipo de un literal o una variable, Python nos ofrece la función `type()`. Veamos algunos ejemplos de su uso:

```python
type(9)
```

Output: `int`

```python
type(1.2)
```

Output: `float`

```python
height = 3718
type(height)
```

Output: `int`

```python
sound_speed = 343.2
type(sound_speed)
```

Output: `float`

O bien, podemos sobreescribir la variable que teníamos originalmente

```python
x = x + 1
```

Output: 4

---

### Operando con una variable numérica

Una vez hemos guardado un valor numérico en una variable, podemos operar con él:

```python
x = 3
x + 1
```

Output: 4

Incluso podemos guardar ese valor en una nueva variable

```
y = x + 1
y
```

Output: 4

### 🔹 Tipos de Datos Básicos

1. **Enteros (`int`)**
    
    ```python
    edad = 30
    ```
    
2. **Números decimales (`float`)**
    
    ```python
    altura = 1.75
    ```
    
3. **Cadenas de texto (`str`)**
    
    ```python
    saludo = "Hola, mundo"
    ```
    
4. **Booleanos (`bool`)**
    
    ```python
    activo = True
    ```
    

### 🔹 Inspeccionar variables

- `type(variable)` → devuelve el tipo de dato
- `print()` → muestra el valor

```python
x = 10
print(type(x))  # <class 'int'>
```

### 🔹 Conversión de tipos (casting)

```python
# Entero a flotante
numero = 5
print(float(numero))  # 5.0

# Texto a entero
texto = "123"
print(int(texto))  # 123
```

En Python, si queremos sobreescribir una variable numérica sumándole esta una cantidad, lo podemos hacer del siguiente modo:

```python
x = 7
x
```

Output: 7

```python
x += 2
x
```

Output: 9

> **Observaciones .** Al igual que existe `+=`, también tenemos `-=`, `*=`, `/=`, `//=`, `%=`, `**=`, `&=`, que son el equivalente a `=` con el resto de operaciones aritméticas existentes en Python y que trataremos en el siguiente tema.
> 

# Práctica 2.

> Entregar todos los ejercicios propuestos de esta clase en un archivo con nombre practica_02.ipynb.
> 
1. Asigna un valor entero 2001 a la variable `space_odyssey` y muestra su valor.
2. Descubre el tipo del literal 'Good night & Good luck'.
3. Identifica el tipo del literal True.
4. Asigna la expresión 10 * 3.0 a la variable `result` y muestra su tipo.

## 📝 5. Ejercicios resueltos:

> Ejecutar los siguientes códigos. Modifícalos cambiando los datos
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