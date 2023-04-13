---
Tema: Resumen
Curso: I
Orden: 0
---


# Python

- PEP8: Guía que indica las convenciones estilísticas a seguir para escribir código Python1. PEP significa Python Enhancement Proposal, que son documentos que proponen mejoras o cambios en el lenguaje Python2. La PEP8 se trata de un conjunto de recomendaciones cuyo objetivo es ayudar a escribir código más legible y consistente entre programas de distintos usuario
    - **Reglas de indentación**
        - Se recomienda indentar usando 4 espacios, dado que los espacios ocupan el mismo tamaño en casi todos los tipos de fuente y 4 es un número aceptable para la separación visual de los bloques.
    - **Reglas de longitud de línea**
        - Se recomienda limitar la longitud de las líneas a 79 caracteres, para facilitar la lectura y evitar el desplazamiento horizontal .
    - **Reglas de espacios en blanco**
        - Se recomienda usar espacios en blanco para separar operadores y operandos, así como para separar las comas, los dos puntos y los puntos y coma de lo que les sigue . No se recomienda usar espacios en blanco alrededor de paréntesis, corchetes o llaves .
    - **Reglas de comentarios**
        - Se recomienda usar comentarios para explicar el código cuando sea necesario, pero evitando comentarios innecesarios o contradictorios. Los comentarios deben ser claros y concisos, y seguir el mismo estilo que el código .
    - **Reglas de nombres**
        - Se recomienda usar nombres descriptivos y consistentes para las variables, funciones, clases, módulos y paquetes . Se recomienda usar minúsculas con guiones bajos para las variables y funciones, mayúsculas con guiones bajos para las constantes, y mayúsculas con minúsculas para las clases .
- Variables: son nombres que se usan para referirse a valores que se pueden almacenar, modificar y recuperar. Por ejemplo:
    
    ```
    x = 10 # asigna el valor 10 a la variable x
    y = "Hola" # asigna el valor "Hola" a la variable y
    z = x + 5 # asigna el valor 15 a la variable z
    
    ```
    
- Tipos de datos: son las categorías que clasifican los valores según sus características y operaciones. [Los tipos de datos básicos en Python son los numéricos (enteros, reales y complejos), las cadenas de texto y los booleanos**2**](https://softwarecrafters.io/python/tutorial-de-python-introduccion/). Por ejemplo:
    
    ```
    a = 42 # tipo entero
    b = 3.14 # tipo real
    c = 1 + 2j # tipo complejo
    d = "Python" # tipo cadena
    e = True # tipo booleano
    
    ```
    
- Control de flujo: son las instrucciones que determinan el orden en que se ejecutan las acciones según ciertas condiciones o repeticiones. [Las principales estructuras de control de flujo en Python son las sentencias if, elif y else para las condiciones, y las sentencias for y while para los bucles**1**](https://docs.python.org/es/3/tutorial/). Por ejemplo:
    
    ```
    if x > 0: # si x es mayor que cero
        print("x es positivo") # imprime este mensaje
    elif x < 0: # si x es menor que cero
        print("x es negativo") # imprime este mensaje
    else: # si x no es ni mayor ni menor que cero
        print("x es cero") # imprime este mensaje
    
    for i in range(5): # para cada valor de i desde 0 hasta 4
        print(i) # imprime el valor de i
    
    while x < 10: # mientras x sea menor que 10
        x = x + 1 # incrementa x en uno
        print(x) # imprime el valor de x
    
    ```
    
- Estructuras de datos: son formas de organizar y manipular los datos en colecciones. [Las estructuras de datos más comunes en Python son las listas, las tuplas, los diccionarios y los conjuntos**1**](https://docs.python.org/es/3/tutorial/). Por ejemplo:
    
    ```
    lista = [1, 2, 3, 4] # una lista es una secuencia ordenada y mutable de elementos
    tupla = (5, 6, 7, 8) # una tupla es una secuencia ordenada e inmutable de elementos
    diccionario = {"nombre": "Ana", "edad": 25} # un diccionario es una colección no ordenada de pares clave-valor
    conjunto = {9, 10, 11, 12} # un conjunto es una colección no ordenada y sin elementos repetidos
    
    ```
    
- Funciones: son bloques de código que realizan una tarea específica y que se pueden reutilizar. Una función se define con la palabra clave def, seguida del nombre de la función y los parámetros entre paréntesis. Una función puede devolver un valor con la palabra clave return[Ver mas qui e](https://docs.python.org/es/3/tutorial/). Por ejemplo:
    
    ```
    def suma(a, b): # define una función que suma dos números
        return a + b # devuelve el resultado
    
    resultado = suma(3, 4) # llama a la función con los argumentos 3 y 4 y guarda el valor devuelto en la variable resultado
    print(resultado) # imprime el valor de la variable resultado
    
    ```
    
- Archivos en Python:
    - Un archivo en Python es un objeto que nos permite trabajar e interactuar con archivos en nuestros programas de Python1. Los archivos pueden ser de texto o binarios, dependiendo del tipo de datos que contienen2. Para abrir un archivo en Python, usamos la función incorporada open(), que toma como argumentos el nombre del archivo y el modo de apertura (por ejemplo, “r” para leer o “w” para escribir)13. Para cerrar un archivo en Python, usamos el método close() del objeto archivo1. Para leer un archivo en Python, podemos usar diferentes métodos del objeto archivo, como read(), readline() o readlines(), que devuelven una cadena o una lista de cadenas con el contenido del archivo1. Para leer un archivo de manera ordenada, podemos usar un bucle for para iterar sobre las líneas del archivo
    
    ```
    # Abrir un archivo para leer o escribir
    archivo = open("datos.txt", "w") # El modo "w" sobreescribe el contenido del archivo
    # Escribir en el archivo
    archivo.write("Hola mundo\n") # El carácter \n representa un salto de línea
    archivo.write("Este es un ejemplo\n")
    # Cerrar el archivo
    archivo.close()
    # Abrir el archivo para leer
    archivo = open("datos.txt", "r") # El modo "r" permite leer el archivo
    # Leer el contenido del archivo
    contenido = archivo.read() # Devuelve una cadena con todo el texto del archivo
    print(contenido) # Imprime el contenido en la consola
    # Cerrar el archivo
    archivo.close()
    ```
    
- Biblioteca :
    - Una biblioteca es un conjunto de módulos que contienen funciones, clases y variables que se pueden usar en otros programas. Para importar o llamar a una biblioteca en Python, se usa la palabra clave **import** seguida del nombre de la biblioteca. Esto permite acceder a los elementos de la biblioteca usando el nombre de la biblioteca como prefijo
    - Por ejemplo, supongamos que queremos usar la biblioteca **math** que contiene funciones matemáticas. Para importarla, escribimos:
        
        ```
        import math
        
        ```
        
        Para usar una función de la biblioteca, como por ejemplo **sqrt** que calcula la raíz cuadrada de un número, escribimos:
        
        ```
        math.sqrt(25)
        
        ```
        
        Esto devuelve el valor 5.0.
        
        También se puede importar solo una parte de la biblioteca usando la sintaxis **from** … **import**. Por ejemplo, para importar solo la función **sqrt**, escribimos:
        
        ```
        from math import sqrt
        
        ```
        
        Esto permite usar la función sin el prefijo de la biblioteca. Por ejemplo:
        
        ```
        sqrt(25)
        
        ```
        
        Esto también devuelve el valor 5.0.
        

Estas son solo algunas de las bases de Python. [Te recomiendo que consultes el tutorial oficial de Python**1**](https://docs.python.org/es/3/tutorial/) o algún otro recurso en línea para aprender más sobre este lenguaje.


---

![[Python]]