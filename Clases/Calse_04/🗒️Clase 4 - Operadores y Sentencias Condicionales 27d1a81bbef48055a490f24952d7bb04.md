# 🗒️Clase 4 - Operadores y Sentencias Condicionales

## 1. Operadores Aritméticos y Relacionales

### Sintaxis

### Operadores Aritméticos

### Operadores Relacionales

```python
# Operadores básicos
+   # Suma
-   # Resta
*   # Multiplicación
/   # División
//  # División entera 7 // 2 = 3
%   # Módulo (resto)
**  # Potencia
```

```python
==  # Igual a
!=  # Diferente de
>   # Mayor que
<   # Menor que
>=  # Mayor o igual que
<=  # Menor o igual que
```

### Ejemplos Básicos Resueltos

### Ejemplo 1: Operaciones aritméticas básicas

### Ejemplo 2: Comparaciones numéricas

```python
# Operaciones con dos números
a = 15
b = 4

suma = a + b           # 19
resta = a - b          # 11
multiplicacion = a * b # 60
division = a / b       # 3.75
division_entera = a // b # 3
modulo = a % b        # 3
potencia = b ** 2     # 16

print(f"15 + 4 = {suma}")
print(f"15 - 4 = {resta}")
print(f"15 * 4 = {multiplicacion}")
print(f"15 / 4 = {division}")
print(f"15 // 4 = {division_entera}")
print(f"15 % 4 = {modulo}")
print(f"4 ** 2 = {potencia}")
```

```python
# Comparar dos valores
x = 25
y = 30

print(f"x = {x}, y = {y}")
print(f"x == y: {x == y}")  # False
print(f"x != y: {x != y}")  # True
print(f"x > y: {x > y}")    # False
print(f"x < y: {x < y}")    # True
print(f"x >= 25: {x >= 25}") # True
print(f"y <= 30: {y <= 30}") # True
```

### Ejemplo 3: Cálculo de promedio

### Ejemplo 4: Verificación de número par

```python
# Calcular el promedio de tres números
nota1 = 85
nota2 = 92
nota3 = 78

suma_total = nota1 + nota2 + nota3
promedio = suma_total / 3
# promedio = (nota1 + nota2 + nota3)/3
print(f"Notas: {nota1}, {nota2}, {nota3}")
print(f"Suma total: {suma_total}")
print(f"Promedio: {promedio:.2f}")

# Verificar si aprobó (promedio >= 70)
aprobado = promedio >= 70
print(f"¿Aprobó? {aprobado}")
# Modificar incluyendo input()
```

```python
# Determinar si un número es par o impar
numero = 42

residuo = numero % 2
es_par = residuo == 0

print(f"Número: {numero}")
print(f"Residuo al dividir entre 2: {residuo}")
print(f"¿Es par? {es_par}")

# Verificación adicional
es_multiplo_de_3 = numero % 3 == 0
print(f"¿Es múltiplo de 3? {es_multiplo_de_3}")
# Modificar incluyendo input()
```

### Ejercicios para Practicar

### Ejercicio 1: Calculador de edad en días

**Enunciado:** Crea un programa que calcule la edad aproximada en días y horas. Dado que una persona tiene 23 años, calcula cuántos días y horas ha vivido aproximadamente (considera 365 días por año). Verifica si es mayor de edad (>= 18 años).

**Salida esperada:**

```
Edad: 23 años
Días vividos: 8395 días
Horas vividas: 201480 horas
¿Es mayor de edad? True
```

### Ejercicio 2: Conversor de temperatura

**Enunciado:** Desarrolla un programa que convierta 28 grados Celsius a Fahrenheit usando la fórmula F = C * 9/5 + 32. Verifica si la temperatura en Fahrenheit es mayor a 80°F (clima cálido).

**Salida esperada:**

```
Temperatura en Celsius: 28°C
Temperatura en Fahrenheit: 82.40°F
¿Es clima cálido (>80°F)? True
Diferencia con punto de congelación: 50.40°F
```

### Ejercicio 3: Análisis de ventas

**Enunciado:** Calcula las estadísticas de ventas de una tienda. Las ventas de 3 días fueron: $1250, $980, $1430. Calcula el total, el promedio diario y verifica si el promedio supera la meta de $1200.

**Salida esperada:**

```
Ventas día 1: $1250
Ventas día 2: $980
Ventas día 3: $1430
Total de ventas: $3660
Promedio diario: $1220.00
¿Supera la meta diaria ($1200)? True
```

### Ejercicios Propuestos

1. **Calculadora de propinas**: Crea un programa que calcule el 15%, 18% y 20% de propina sobre un monto de cuenta de restaurante.
2. **Conversor de unidades**: Desarrolla un programa que convierta kilómetros a millas, metros y pies.
3. **Calculador de IMC**: Implementa un programa que calcule el Índice de Masa Corporal (IMC = peso / altura²) y determine si está en el rango saludable (18.5 - 24.9).
4. **Verificador de año bisiesto**: Crea un programa que determine si un año es bisiesto (divisible por 4, pero no por 100, excepto si es divisible por 400).
5. **Calculador de descuento**: Desarrolla un programa que calcule el precio final de un producto después de aplicar un descuento porcentual.
6. **Distancia entre puntos**: Implementa un programa que calcule la distancia entre dos puntos en un plano cartesiano usando la fórmula de distancia euclidiana.
7. **Área y perímetro**: Crea un programa que calcule el área y perímetro de un rectángulo dados su base y altura.
8. **Validador de triángulo**: Desarrolla un programa que verifique si tres números dados pueden formar un triángulo válido.
9. **Calculador de interés simple**: Implementa un programa que calcule el interés simple dado el capital, tasa y tiempo.
10. **Comparador de precios**: Crea un programa que compare los precios de tres productos y determine cuál es el más económico y cuál el más caro.

## 2. Operadores Lógicos (and, or, not)

### Sintaxis

### Tabla de Verdad

```python
and  # Y lógico - True si ambos operandos son True
or   # O lógico - True si al menos un operando es True
not  # NO lógico - Invierte el valor booleano
```

```python
# AND
True and True   = True
True and False  = False
False and True  = False
False and False = False

# OR
True or True    = True
True or False   = True
False or True   = True
False or False  = False

# NOT
not True  = False
not False = True
```

### Ejemplos Básicos Resueltos

### Ejemplo 1: Validación de edad y membresía

```python
# Verificar acceso a un club
edad = 21
tiene_membresia = True
acompañado = False

# Puede entrar si: es mayor de edad Y tiene membresía
puede_entrar = edad >= 18 and tiene_membresia
print(f"Edad: {edad}")
print(f"Tiene membresía: {tiene_membresia}")
print(f"¿Puede entrar solo? {puede_entrar}")

# Puede entrar como invitado si: está acompañado O tiene membresía
entrada_permitida = acompañado or tiene_membresia
print(f"¿Entrada permitida? {entrada_permitida}")

# NO es menor de edad
es_mayor = not (edad < 18)
print(f"¿Es mayor de edad? {es_mayor}")
```

### Ejemplo 2: Sistema de aprobación

```python
# Verificar si un estudiante aprueba
nota_teoria = 75
nota_practica = 80
asistencia = 85

# Aprueba si: ambas notas >= 70 Y asistencia >= 80
aprueba_teoria = nota_teoria >= 70
aprueba_practica = nota_practica >= 70
buena_asistencia = asistencia >= 80

aprobado = aprueba_teoria and aprueba_practica and buena_asistencia
print(f"Teoría: {nota_teoria} - Aprobada: {aprueba_teoria}")
print(f"Práctica: {nota_practica} - Aprobada: {aprueba_practica}")
print(f"Asistencia: {asistencia}% - Suficiente: {buena_asistencia}")
print(f"Resultado final: {'APROBADO' if aprobado else 'REPROBADO'}")

# Necesita recuperación si falla teoría O práctica (pero no ambas)
recuperacion = (not aprueba_teoria) or (not aprueba_practica)
print(f"¿Necesita recuperación? {recuperacion}")
```

### Ejemplo 3: Validación de contraseña simple

```python
# Verificar si una contraseña cumple requisitos básicos
password = "Python2024"
longitud = len(password)

# Requisitos
longitud_valida = longitud >= 8
tiene_mayuscula = any(c.isupper() for c in password)
tiene_numero = any(c.isdigit() for c in password)

# Contraseña válida si cumple TODOS los requisitos
es_valida = longitud_valida and tiene_mayuscula and tiene_numero
print(f"Contraseña: {'*' * len(password)}")
print(f"Longitud >= 8: {longitud_valida}")
print(f"Tiene mayúscula: {tiene_mayuscula}")
print(f"Tiene número: {tiene_numero}")
print(f"¿Contraseña válida? {es_valida}")

# NO es una contraseña débil
no_es_debil = not (longitud < 6)
print(f"¿No es débil? {no_es_debil}")
```

### Ejercicios para Practicar

### Ejercicio 1: Acceso a biblioteca

**Enunciado:** Un sistema de biblioteca verifica el acceso. Un usuario tiene carnet válido (True), no tiene multas (True), y es horario de atención (False). Puede acceder si: tiene carnet Y no tiene multas. Acceso especial si es investigador (True) O es horario de atención. Verificar también si NO está vetado del sistema.

**Salida esperada:**

```
Carnet válido: True
Sin multas: True
Horario de atención: False
Es investigador: True
Acceso normal: True
Acceso especial: True
¿No está vetado? True
Estado: ACCESO PERMITIDO
```

### Ejercicio 2: Evaluación de beca

**Enunciado:** Para otorgar una beca se evalúa: promedio = 88, ingresos familiares = $35000, es deportista = False. Califica si: promedio >= 85 Y ingresos < 40000. Beca especial si: es deportista O promedio >= 90. Verificar si NO supera el límite de ingresos ($50000).

**Salida esperada:**

```
Promedio: 88
Ingresos familiares: $35000
Es deportista: False
Califica beca regular: True
Califica beca especial: False
No supera límite de ingresos: True
Decisión: BECA REGULAR OTORGADA
```

### Ejercicio 3: Sistema de alerta

**Enunciado:** Un sistema de seguridad tiene: sensor de movimiento (True), puerta cerrada (False), es horario nocturno (True). Activar alarma si: movimiento Y puerta abierta (not cerrada). Modo vigilancia si: horario nocturno O sensor activo. Sistema armado si: puerta cerrada Y NOT hay movimiento es False.

**Salida esperada:**

```
Sensor de movimiento: True
Puerta cerrada: False
Horario nocturno: True
Activar alarma: True
Modo vigilancia: True
Sistema armado: False
Estado: ALARMA ACTIVADA
```

### Ejercicios Básicos Propuestos

1. **Validador de formulario**: Crea un programa que valide si un formulario está completo verificando que el nombre no esté vacío, el email contenga “@” y la edad sea mayor a 18.
2. **Sistema de descuento**: Desarrolla un programa que aplique descuento si: es cliente frecuente Y compra > $100, O si es día de promoción.
3. **Control de calidad**: Implementa un sistema que apruebe un producto si: peso correcto Y medidas correctas Y NOT tiene defectos.

## 3. Sentencias Condicionales: if, elif, else

### Sintaxis

```python
# Estructura básica if
if condicion:
    # Código si la condición es True
    instrucciones

# Estructura if-else
if condicion:
    # Código si la condición es True
    instrucciones
else:
    # Código si la condición es False
    otras_instrucciones

# Estructura if-elif-else
if condicion1:
    # Código si condicion1 es True
    instrucciones1
elif condicion2:
    # Código si condicion2 es True
    instrucciones2
elif condicion3:
    # Código si condicion3 es True
    instrucciones3
else:
    # Código si ninguna condición es True
    instrucciones_por_defecto
```

### Ejemplos Básicos Resueltos

### Ejemplo 1: Clasificación de calificaciones

```python
# Determinar la letra de calificación según el puntaje
puntaje = 78

if puntaje >= 90:
    calificacion = "A"
    mensaje = "Excelente"
elif puntaje >= 80:
    calificacion = "B"
    mensaje = "Muy bien"
elif puntaje >= 70:
    calificacion = "C"
    mensaje = "Bien"
elif puntaje >= 60:
    calificacion = "D"
    mensaje = "Suficiente"
else:
    calificacion = "F"
    mensaje = "Insuficiente"

print(f"Puntaje: {puntaje}")
print(f"Calificación: {calificacion}")
print(f"Resultado: {mensaje}")
```

### Ejemplo 2: Categoría por edad

```python
# Clasificar a una persona según su edad
edad = 15

if edad < 0:
    categoria = "Error: edad inválida"
elif edad < 12:
    categoria = "Niño"
elif edad < 18:
    categoria = "Adolescente"
elif edad < 60:
    categoria = "Adulto"
else:
    categoria = "Adulto mayor"

print(f"Edad: {edad} años")
print(f"Categoría: {categoria}")

# Determinar si puede votar
if edad >= 18:
    print("Puede votar: Sí")
else:
    print("Puede votar: No")
```

### Ejemplo 3: Calculadora de descuento

```python
# Aplicar descuento según el monto de compra
monto_compra = 75

if monto_compra >= 100:
    descuento = 15  # 15%
elif monto_compra >= 50:
    descuento = 10  # 10%
elif monto_compra >= 25:
    descuento = 5   # 5%
else:
    descuento = 0   # Sin descuento

monto_descuento = monto_compra * (descuento / 100)
total_pagar = monto_compra - monto_descuento

print(f"Monto original: ${monto_compra}")
print(f"Descuento aplicado: {descuento}%")
print(f"Ahorro: ${monto_descuento:.2f}")
print(f"Total a pagar: ${total_pagar:.2f}")
```

### Ejercicios para Practicar

### Ejercicio 1: Estado del agua

**Enunciado:** Crea un programa que determine el estado del agua según la temperatura. Para una temperatura de -5°C, indica si es: hielo (<0°C), líquido (0-100°C), o vapor (>100°C). También indica si es temperatura ambiente (15-25°C).

**Salida esperada:**

```
Temperatura: -5°C
Estado del agua: Hielo
¿Temperatura ambiente? No
Recomendación: Temperatura bajo cero, riesgo de congelamiento
```

### Ejercicio 2: Tarifas de estacionamiento

**Enunciado:** Calcula el costo de estacionamiento para 5 horas. Tarifa: 1 hora = $3, 2-3 horas = $2.50/hora, 4-6 horas = $2/hora, más de 6 horas = tarifa fija de $15. Indica si es estancia corta (<2 horas), media (2-4 horas) o larga (>4 horas).

**Salida esperada:**

```
Tiempo estacionado: 5 horas
Tarifa aplicada: $2.00 por hora
Costo total: $10.00
Tipo de estancia: Larga
```

### Ejercicio 3: Clasificador de IMC

**Enunciado:** Calcula el IMC para una persona de 70 kg y 1.75 m. Clasifica según: <18.5 = Bajo peso, 18.5-24.9 = Normal, 25-29.9 = Sobrepeso, >=30 = Obesidad. Proporciona una recomendación básica.

**Salida esperada:**

```
Peso: 70 kg
Altura: 1.75 m
IMC: 22.86
Clasificación: Normal
Recomendación: Mantener hábitos saludables
```

### Ejercicios Propuestos

1. **Calculadora de envío**: Crea un programa que calcule el costo de envío según el peso del paquete con diferentes tarifas por rango de peso.
2. **Sistema de notas**: Desarrolla un programa que convierta una nota numérica (0-100) a su equivalente literal.
3. **Clasificador de triángulos**: Implementa un programa que determine si un triángulo es equilátero, isósceles o escaleno.
4. **Selector de plan telefónico**: Crea un programa que recomiende un plan según el consumo mensual de minutos.
5. **Evaluador de presión arterial**: Desarrolla un programa que clasifique la presión arterial en normal, elevada, o hipertensión.

## 4. Uso Combinado con Operadores

### Ejemplos Básicos Resueltos

### Ejemplo 1: Sistema de login

```python
# Sistema simple de autenticación
usuario = "admin"
password = "1234"
intentos = 2

# Credenciales correctas
usuario_correcto = usuario == "admin"
password_correcta = password == "1234"
intentos_restantes = 3 - intentos

# Verificar acceso
if usuario_correcto and password_correcta:
    print("Acceso permitido")
    print("Bienvenido al sistema")
elif not usuario_correcto:
    print("Usuario incorrecto")
    print(f"Intentos restantes: {intentos_restantes}")
elif not password_correcta:
    print("Contraseña incorrecta")
    print(f"Intentos restantes: {intentos_restantes}")
    
# Bloquear después de 3 intentos
if intentos >= 3:
    print("Cuenta bloqueada temporalmente")
```

### Ejemplo 2: Evaluación de crédito simple

```python
# Evaluar elegibilidad para crédito
edad = 28
ingresos = 3500
historial_crediticio = True
deudas_actuales = 500

# Calcular capacidad de pago
capacidad_pago = ingresos - deudas_actuales
porcentaje_disponible = (capacidad_pago / ingresos) * 100

# Criterios
es_mayor = edad >= 21
buenos_ingresos = ingresos >= 2000
buen_historial = historial_crediticio
capacidad_suficiente = capacidad_pago >= (ingresos * 0.3)

# Evaluación
if es_mayor and buenos_ingresos and buen_historial and capacidad_suficiente:
    estado = "APROBADO"
    limite = ingresos * 3
elif es_mayor and buenos_ingresos and not buen_historial:
    estado = "APROBADO CON CONDICIONES"
    limite = ingresos * 1.5
else:
    estado = "RECHAZADO"
    limite = 0

print(f"Edad: {edad} años")
print(f"Ingresos: ${ingresos}")
print(f"Capacidad de pago: {porcentaje_disponible:.1f}%")
print(f"Estado de solicitud: {estado}")
if limite > 0:
    print(f"Límite de crédito: ${limite:.2f}")
```

### Ejemplo 3: Sistema de calificación con bonus

```python
# Calcular nota final con bonificaciones
nota_examenes = 75
nota_tareas = 85
nota_participacion = 90
asistencia = 92

# Calcular promedio base
promedio_base = (nota_examenes * 0.5) + (nota_tareas * 0.3) + (nota_participacion * 0.2)

# Aplicar bonus por asistencia
if asistencia >= 95:
    bonus = 5
elif asistencia >= 90:
    bonus = 3
elif asistencia >= 85:
    bonus = 1
else:
    bonus = 0

nota_final = min(promedio_base + bonus, 100)  # Máximo 100

# Determinar estado
if nota_final >= 90 and asistencia >= 90:
    estado = "EXCELENTE"
    mencion = "Con honores"
elif nota_final >= 80:
    estado = "MUY BUENO"
    mencion = "Felicitaciones"
elif nota_final >= 70:
    estado = "APROBADO"
    mencion = "Satisfactorio"
else:
    estado = "REPROBADO"
    mencion = "Debe repetir"

print(f"Promedio base: {promedio_base:.1f}")
print(f"Bonus por asistencia: +{bonus}")
print(f"Nota final: {nota_final:.1f}")
print(f"Estado: {estado}")
print(f"Observación: {mencion}")
```

### Ejercicios para Practicar

### Ejercicio 1: Sistema de membresía de gimnasio

**Enunciado:** Calcula el costo de membresía mensual. Datos: edad = 35, es_estudiante = False, meses_contrato = 6, horario_premium = True. Tarifa base: $40. Descuentos: estudiantes 20%, mayores de 60 años 25%, contrato 6+ meses 10%. Recargo horario premium: 15%. Si el total con descuentos es menor a $30, aplicar tarifa mínima de $30.

**Salida esperada:**

```
Edad: 35 años
Tipo: Regular
Contrato: 6 meses
Horario: Premium
Tarifa base: $40.00
Descuento por contrato: -$4.00
Recargo premium: +$5.40
Total mensual: $41.40
Total contrato (6 meses): $248.40
```

### Ejercicio 2: Evaluador de rendimiento laboral

**Enunciado:** Evalúa a un empleado con: puntualidad = 95, productividad = 88, trabajo_equipo = 92, años_empresa = 3, certificaciones = 2. Promedio ponderado: puntualidad 20%, productividad 50%, trabajo_equipo 30%. Si promedio >= 90 Y años >= 2 = “Promoción”. Si promedio >= 80 O certificaciones >= 2 = “Aumento”. Si promedio < 70 = “Capacitación”.

**Salida esperada:**

```
=== EVALUACIÓN DE DESEMPEÑO ===
Puntualidad: 95
Productividad: 88
Trabajo en equipo: 92
Promedio ponderado: 90.10
Años en empresa: 3
Certificaciones: 2
Resultado: PROMOCIÓN
Recomendación: Candidato a líder de equipo
Aumento salarial: 15%
```

### Ejercicio 3: Sistema de alerta de salud

**Enunciado:** Monitorea signos vitales: frecuencia_cardiaca = 105, presion_sistolica = 135, temperatura = 37.8, oxigeno = 94. Normal: FC 60-100, presión <120, temp 36-37.5, O2 >95. Si 2 o más valores anormales = “Alerta Amarilla”. Si FC > 120 O presión > 140 O O2 < 90 = “Alerta Roja”. Si todos normales = “Estado óptimo”.

**Salida esperada:**

```
=== MONITOREO DE SIGNOS VITALES ===
Frecuencia cardíaca: 105 bpm - Elevada
Presión sistólica: 135 mmHg - Elevada
Temperatura: 37.8°C - Febrícula
Oxígeno: 94% - Bajo
Valores anormales: 4
Estado: ALERTA AMARILLA
Recomendación: Consultar con médico
Signos a vigilar: FC, Presión, Temperatura
```

### Caso de Uso Propuesto

**Sistema de Gestión de Reservas Hoteleras**

Desarrollar un sistema que gestione reservas de hotel considerando:

**Datos de entrada:**

- Tipo de habitación (Simple, Doble, Suite)
- Número de noches
- Temporada (Alta, Media, Baja)
- Es fin de semana (Sí/No)
- Cliente frecuente (Sí/No)
- Cantidad de huéspedes
- Servicios adicionales (Desayuno, Spa, Parking)
- Edad del cliente principal

**Reglas de negocio:**

1. Tarifas base por noche:
    - Simple: $50
    - Doble: $75
    - Suite: $120
2. Modificadores de precio:
    - Temporada alta: +30%
    - Temporada media: +10%
    - Fin de semana: +20%
    - Cliente frecuente: -10%
3. Validaciones:
    - Simple: máximo 2 huéspedes
    - Doble: máximo 4 huéspedes
    - Suite: máximo 6 huéspedes
    - Menores de 18 no pueden hacer reservas
4. Servicios adicionales:
    - Desayuno: $10 por persona por noche
    - Spa: $30 por día
    - Parking: $15 por noche
5. Descuentos especiales:
    - Estancia 7+ noches: 5% adicional
    - Estancia 14+ noches: 10% adicional
    - Mayores de 65 años: 5% adicional

**Salida esperada:**

```
- Estado de la reserva (Aprobada/Rechazada)
- Motivo del rechazo (si aplica)
- Desglose de costos
- Total antes de descuentos
- Descuentos aplicados
- Total final
- Políticas de cancelación según el tipo de reserva
```

---