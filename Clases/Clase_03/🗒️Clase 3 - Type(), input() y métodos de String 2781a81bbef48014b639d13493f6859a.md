# 🗒️Clase 3 - Type(), input() y métodos de String

# **Variables y Tipos de Datos**

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

```python
Output: 9
```

> **Observaciones .** Al igual que existe `+=`, también tenemos `-=`, `*=`, `/=`, `//=`, `%=`, `**=`, `&=`, que son el equivalente a `=` con el resto de operaciones aritméticas existentes en Python y que trataremos en el siguiente tema.
> 

## 🔹 Tipos de Datos Básicos

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

## 🔹 Conversión de tipos (casting)

```python
# Entero a flotante
numero = 5
print(float(numero))  # 5.0

# Texto a entero
texto = "123"
print(int(texto))  # 123
```

## Constantes

Las constantes también se componen de un nombre y de un valor. En otros lenguajes de programación, a diferencia de las variables, su valor no se puede modificar. Se utilizan para establecer valores que son de uso común y que no se deberían modificar a lo largo del código. Por ejemplo, podríamos utilizar una constante para almacenar el valor del IVA.

Como Python no posee una declaración especial para crear una constante, una buena práctica es crear un archivo .py separado que contenga solo las constantes y sus valores asignados. Luego este archivo se puede importar dentro de nuestro código para hacer uso de las constantes declaradas.

Para diferenciar una constante de una variable, por convención el nombre de la constante se escribe completamente en mayúsculas.

```python
IVA = 0.18
NUMERO_PI = 3.14
```

### Algunos ejemplos de asignaciones a constantes:

```python
SOUND_SPEED = 343.2
WATER_DENSITY = 997
EARTH_NAME = 'La Tierra'
```

# Strings y métodos asociados

¿Qué obtendremos al "sumar" dos Strings?

```python
a = 'HOLA'
b = 'MUNDO'
print(a + b)
```

```
HOLA MUNDO
```

> **Al asignar los valores utilizando comillas simples, Python los interpreta como String. Por ende, la instrucción dada por el carácter `+`, para este caso, es de concatenar, no de sumar.**
> 

En programación, la acción de 'sumar' dos o más Strings se conoce como *concatenación*.

## Concatenación

Podemos obtener los mismo resultados utilizando concatenación e interpolación, sin embargo, se prefiere la interpolación debido a que es más rápida y presenta una sintaxis más amigable para el desarrollador.

```python
nombre = 'Carlos'
apellido = 'Santana'
# Concatenación
print("Mi nombre es " + nombre + " " + apellido)
```

```
Mi nombre es Carlos Santana
```

## Interpolación

Otra acción muy importante y ampliamente utilizada al momento de trabajar con Strings es la interpolación.

La interpolación es un mecanismo que nos permite introducir una variable (o un dato) dentro un String, sin necesidad de concatenarlo. Para interpolar simplemente tenemos que introducir la variable (o dato) utilizando la siguiente notación:

```python
nombre = 'Carlos'
apellido = 'Santana'
# Interpolación
print("Mi nombre es {} {}".format(nombre, apellido))
```

```
Mi nombre es Carlos Santana
```

## Count

Otro método que se puede aplicar a las variables de tipo string es `count`, que nos permite contar la cantidad de ocurrencias de un carácter específico dentro de un texto.

En este caso, al hacer:

```python
print(nombre.count("a"))
```

```
Obtenemos como resultado "1", porque la letra "a" aparece 1 vez en el texto "Carlos".
```

## Len

Entrega la cantidad de letras o el "largo" del texto. Por tanto al ejecutar:

```python
print(len(apellido))
```

```
Se obtiene 7, que es la cantidad de letras de "Santana".
```

## Upper

Aplica letras mayúsculas a todo el texto:

```python
print(apellido.upper())
```

```
SANTANA
```

## Ejercicios para practicar (15 minutos)

<aside>

### Ejercicio 1: Constantes en Python

Crea un programa en Python que defina una constante llamada `GRAVEDAD` con el valor 9.81 y la utilice para imprimir un mensaje que diga "La gravedad es GRAVEDAD m/s²".

### Ejercicio 2: Concatenación

Concatena tu nombre y apellido usando el operador `+` e imprímelo en una sola línea con un espacio entre ellos.

### Ejercicio 3: Interpolación

Use el método `.format()` para interpolar tu edad y nombre en la frase "Me llamo {nombre} y tengo {edad} años".

### Ejercicio 4: Count, Len y Upper

Crea un programa en Python que tome una palabra, cuente las veces que aparece la letra "a" con `.count("a")`, obtenga su longitud con `len()`, y la convierta a mayúsculas con `.upper()`.

</aside>

# El salto de línea en un string

El salto de línea `\n` es un caracter especial que nos permite agregar un salto de línea dentro de un string. 

```python
saltos = "hola\na\ntodos"
print(saltos)
```

```
hola
a
todos
```

### Tabulación horizontal  \t  (horizontal tab)

```python
print("Hello\tWorld")
```

```
Hello    World
```

## Ejercicios para practicar (10 minutos)

<aside>

### Ejercicio 5: Salto de línea simple

Imprime tu nombre completo utilizando el carácter de salto de línea (\n) para separar el nombre y el apellido en líneas diferentes.

### Ejercicio 6: Combinación de salto y tabulación

Imprime una lista de tareas donde cada tarea esté precedida por un carácter de tabulación (\t) y las tareas estén separadas por un salto de línea (\n).

</aside>

# La función `input()` y entrada de datos por teclado en Python

---

La función `input()` en Python permite que un programa reciba datos ingresados por el usuario a través del teclado. Es una herramienta fundamental para hacer que los programas sean interactivos.

- **Sintaxis básica**:
    
    ```python
    variable = input("Mensaje para el usuario: ")
    
    ```
    
- El mensaje dentro de `input()` se muestra en pantalla para guiar al usuario.
- Todo lo que el usuario ingresa se almacena como una **cadena de texto** (string) en la variable.

**Ejemplo 1**:

```python
nombre = input("¿Cuál es tu nombre? ")
print("¡Hola, " + nombre + "!")
```

**Salida** (si el usuario ingresa "Ana"):

```
¿Cuál es tu nombre? Ana
¡Hola, Ana!
```

> **Punto clave**: La función `input()` siempre devuelve un string, incluso si el usuario ingresa números. Si necesitas un número, debes convertirlo.
> 

---

## Conversión de tipos de datos

Cuando el usuario ingresa un número, `input()` lo trata como texto. Para usar ese valor como número, necesitamos convertirlo a un tipo numérico (`int` o `float`).

- `int()`: Convierte a un número entero.
- `float()`: Convierte a un número decimal.

**Ejemplo 2: Entrada de números**:

```python
edad = int(input("¿Cuántos años tienes? "))
print("El próximo año tendrás", edad + 1, "años.")
```

**Salida** (si el usuario ingresa "15"):

```
¿Cuántos años tienes? 15
El próximo año tendrás 16 años.
```

**Ejemplo 3: Trabajando con decimales**:

```python
altura = float(input("¿Cuál es tu altura en metros? "))
print("Tu altura es", altura, "metros.")
```

**Salida** (si el usuario ingresa "1.75"):

```
¿Cuál es tu altura en metros? 1.75
Tu altura es 1.75 metros.
```

## Ejemplos prácticos

### Ejemplo 4: Calculadora simple

Este programa pide dos números y calcula su suma.

```python
numero1 = float(input("Ingresa el primer número: "))
numero2 = float(input("Ingresa el segundo número: "))
suma = numero1 + numero2
print("La suma es:", suma)
```

**Salida** (si el usuario ingresa "3.5" y "2.5"):

```
Ingresa el primer número: 3.5
Ingresa el segundo número: 2.5
La suma es: 6.0
```

### Ejemplo 5: Personalizando mensajes

Este programa combina varios datos ingresados por el usuario.

```python
nombre = input("¿Cuál es tu nombre? ")
hobby = input("¿Cuál es tu pasatiempo favorito? ")
print(nombre, "disfruta de", hobby, "en su tiempo libre.")

```

**Salida** (si el usuario ingresa "Carlos" y "jugar fútbol"):

```
¿Cuál es tu nombre? Carlos
¿Cuál es tu pasatiempo favorito? jugar fútbol
Carlos disfruta de jugar fútbol en su tiempo libre.

```

---

## Ejercicios para practicar (15 minutos)

<aside>

### Ejercicio 7: **Saludo personalizado**

Escribe un programa que pida al usuario su nombre y su ciudad, y luego muestre un mensaje como:

`"¡Hola, [nombre]! Bienvenido/a desde [ciudad]."`.

### Ejercicio 8: **Calculadora de edad**

Escribe un programa que pida al usuario su edad, la convierta a un número entero y muestre cuántos años tendrá dentro de 5 años.

</aside>

## 🔄 Tipos de Conversión de Datos

| Función | Descripción | Ejemplo |
| --- | --- | --- |
| `str()` | Convierte a texto (por defecto) | `"123"` |
| `int()` | Convierte a número entero | `123` |
| `float()` | Convierte a número decimal | `123.45` |
| `bool()` | Convierte a verdadero/falso | `True/False` |

# 🔄 Conversión con bool()

## Ejemplo 1: Comportamiento básico de bool()

```python
# bool() convierte strings a True/False
respuesta = input("¿Te gusta Python? (escribe algo): ")
es_verdadero = bool(respuesta)

print(f"Tu respuesta: '{respuesta}'")
print(f"Convertido a bool: {es_verdadero}")
```

**Comportamiento de bool() con strings:**

- **String vacío** `""` → `False`
- **Cualquier string con contenido** → `True`

---

---

## Ejemplo 2: Conversión de números a booleano

```python
numero = input("Ingresa un número: ")
numero_entero = int(numero)
es_verdadero = bool(numero_entero)

print(f"Número: {numero_entero}")
print(f"Como booleano: {es_verdadero}")
```

**Comportamiento de bool() con números:**

- `0` → `False`
- **Cualquier otro número** (positivo o negativo) → `True`

---

## 🔍 Puntos Clave sobre bool():

1. **String vacío** = `False`
2. **Cualquier string con contenido** = `True` (incluso `"0"` o `"False"`)
3. **Número 0** = `False`
4. **Cualquier otro número** = `True`
5. Es útil para **validar si el usuario ingresó algo**

---

## Ejercicios para practicar (15 minutos)

<aside>

### Ejercicio 9: **Convertir número a booleano**

Escribe un programa que pida al usuario un número entero y un decimal luego que use bool() para convertirlos a booleano. Muestra los números ingresados y su valor booleano.

### Ejercicio 10: Verificador de Datos

Crea un programa que solicite diferentes tipos de información al usuario y muestre cómo se comporta la conversión `bool()` con cada entrada.

### Instrucciones:

1. Solicita al usuario que ingrese su **nombre** (puede dejarlo vacío)
2. Solicita que ingrese su **edad** como número
3. Solicita que ingrese un **comentario** sobre Python (puede dejarlo vacío)
4. Para cada entrada, muestra:
    - El valor original que ingresó
    - El resultado de convertirlo con `bool()`
    - Un mensaje explicativo sobre el resultado

Ejemplo de salida esperada:

```
Ingresa tu nombre (puedes dejarlo vacío): María
Ingresa tu edad: 25
Escribe un comentario sobre Python (puedes dejarlo vacío): 

=== RESULTADOS DE CONVERSIÓN bool() ===
Nombre: 'María' → True
Edad: 25 → True
Comentario: '' → False

=== EXPLICACIÓN ===
Tu nombre tiene contenido
Tu edad 25 es diferente de cero
Tu comentario está vacío
```

</aside>