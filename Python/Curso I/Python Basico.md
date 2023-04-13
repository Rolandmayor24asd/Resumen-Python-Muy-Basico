---
Tema: Inicio de Programación 
Curso: I
Orden: 2
Clases: 2
---


# Detalles de terminar del IDE y de la escritura de  python

Python usa la extensión **.py** creandose en base de un .text (o puede crearse desde el IDE como visual estudio)

El IDE brinda ayuda para programar por su especialidad del mismo teniendo 3 ayudas visuales 

>	- Rojo: Un error grave, palabras que no existen en el código base
>	- Amarillo: Advertencia
>	- Bombillo es una sugerencia

# PEP 8

Estandar de como escribir Python como codigo de manera ordenada y leible para todos: 

Este viende de manera oficial en su pagina: [https://www.python.org/dev/peps/pep-0008/](https://www.python.org/dev/peps/pep-0008/)

Siendo este un tema opcional tenemos obligatorio: 

- **La identación** 
	- Espacios/tabulador de cada codigo, preferible usar 4 espacios de identación y evitar el tabulador (menos combinar)

- **Limite de caracteres por linea**
	- Este es de 79 como máximo y si fallas divides la linea con las:
	- “,” o “\” (alt+92) 

- **Espacio entre  lineas diferentes**
	- Este se deja normalmente 2, pero si ocupas mas no hay problema

- **Quotes** 
	- La hilera de texto o String siempre vendran en “ o ‘
	- Estas nunca vendran combinadas
	- Y al ojo del interprete da igual cual de los dos uses

```python
print("Hola Mundo :D, Este es mi primer texto")
print('01010011,01101111,01101100')
```

- **Dar comentarios**
	- Este se usa el numeral `#` y esto no afecta el codigo cuando es en la misma linea, pero para hacer un comentario en bloque se usa tres veces las dobles comillas


```python

#Comentario en linea

print("Hola Mundo :D") #comentario en linea

"""
Esto es un comentario en bloque donde van entre 6 comillas dobles
"""
```

- **Reglas de variable** 
	- No puede iniciar con un numero (solo con una letra o guion bajo)
	- No puede ser entre comillas 
	- No puede tener espacio en el nombre
	- Guion bajo para separar o mayuscula en cada palabra
	- Evitar caracteres especiales (tildes/ñ)
	- Por tema de lecturas 
		- Desde 0-9 sin iniciar, las 26 letras y guion bajo (_)

[[Python Resumen#Python]]

# Lineas basicas de programación

## Comandos del cmd

| dir | Para ver que carpetas tienes |
| --- | --- |
| cls | Un “clear” |
| cd.. | Ir atras (cuadno estes abajo poner c:/d: |
| cd | Nombre de carpeta/ver la ruta |
| exit | Salir |
| copy | Copia archivo de la ruta destino |
| move | Mueve archivo de la ruta destino  |
| ctrl + c | Finaliza ejecución de programa |

## Lienas basicas de Python

### **El “print”**

Su función es para imprimir una hilera de texto, numero o variable en la consola. Para poner un numero decimal es con “.”  y si quiero agregar otra frase pongo “,” brindando automáticamente un espacio.

```python
print("Hola mundo",
    "bienvenido a Python",
    "por que hablamos de esta manera?" )
print("mira como se siente ser un",-1.1)
print("EL RESULTADO de la operación", "23+24", "es", 23+24)
```

### **Las variables**

Estos son contenedores vacios que se decide relacionar algo con esta temporalmente (en la ram). Este viene por nombres y nunca van en comillas, definiendose como:

```python
equipo = "Saprisa"
```

Donde equipo es igual a la variable y en su interior se usa saprisa.

Las variables pueden ser reescritas y borradas (con “del”) dentro del mismo codigo mas adelante, ejemplo que equipo cambie por otro 

```python
#aqui las variable
equipo = "Saprisa" #aqui asigno la palabra equipo a la variable Saprisa
#ejemplo del uso de la variante 
print( equipo ) #debes asiganar primero la variable
#reescribo la variable
equipo = "C.S.Cartaginés"
#Imprimo otro resultado 
print( equipo )
```

### **El “input”**

Es la forma de Python para pedir la información al usuario, pudiendo ser usada en las variables como ejemplo 

```python
#ponemos input para solicitar al usuario la palabra
vive = input("digite su provincia de residencia para determinar en que hospital deberías ir")
#imprime el texto + la variable tenga guardado :D
print("El usuario debe ir al hospital de", vive)
```

### **Operadores aritméticos**

Las operaciones basicas son admitidas por Python directamente (+ - / * %) 

### **Operadores de Asignación** 

Forma de acortar el codigo, permiten realizar una operación y almacenar su resultado en la variable inicial, con los ejemplos 

```python
a = 0

a += 5 #suma en asignación
a -= 5 #resta en asignaicón 
a *= 5 #multplica en asiganción 
a /= 5 #división en asignación 
a **= 5 #potencia en asignación  
a %= 5 #modulo de asignación 
```

![[Python]]