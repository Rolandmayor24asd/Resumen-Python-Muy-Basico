---
Tema: Datos
Curso: I
Orden: 3
Clases: 3
---


# Tipos de datos

Tipos de datos primitivos

					(Codigos que ya vienen con Python)

## **La hilera (string)**

El que se puede **escribir cualquier formación escrita** 

```python
“Esto es un Stringer”
```

> El comando input siempre es considerado un string

## **Numeros enteros (Integer)**

Todos los numeros **sin la parte decimal**

```python
int() #su forma de representaicón en Python
```

## **Punto flotante (Float)**

Todos los **decimales** despues de un punto “.”

```python
float() #su forma de representaicón en Python
```

## **Booleano (Boolean)**

Es el **True, False, 0, 1** (el on y off de toda la vida)

```python
bool() #su forma de representaicón en Python
```

## **Nada (None)**

None (literalmente nada)

```python
None # Se puede decir que la variable esta vacio 
```


### Dato importante

> Python es fuertemente tipado, donde string es string entonces 10.0 + 10 no es posible


# Conversiones

![Untitled](Curso%20I/Continuación%20de%20Python%20Basico/Untitled.png)

1. **Entre numeros** 

> Entero → Flotante

```python
float(x) #lo convierte en x.0 (poniendolo en el print)
print(float(x))
```

> Flotantes → Enteros 

```python
int(x) #le quita los desimales "SIN REDONDEAR" 
```

2. **Cadenas a numeros**

>Numero → Cadena

```python
str(12) #en la terminal convierte 12 en "12" en el  output
```

-  Usado para poder usar el numero en el texto sin dar error, podemos realizar una prueba para asegurarnos de que esté bien, realizando una concatenación con una cadena.

>Cadena → Numero

```python
lines_yesterday = "50"
lines_today = "108"

lines_more = int(lines_today) - int(lines_yesterday)

print(lines_more)
```

Pero no podemos convertir los numeros en el mismo codigo 

```python
f = "54.23"
print(int(f))#Si pasamos un valor decimal en una cadena al método int(), obtendremos un error porque no se convertirá en un entero.
"""
ValueError: invalid literal for int() with base 10: '54.23'
"""
```

3. **Los Booleanos a otros** 

```python
bool() #su forma de representaicón en Python
```

4. **Tuplas y Listas (no estudiado)**

Las listas es una secuencia ordenada de elementos mutables contenidas entre corchetes “[]” y la tupla es la secuancia oredenada de elementos inmutables contenida entre paréntesis “()” mas especifico

Las listas son elementos cambiable en secuencia ordenada, estos son definidos entre comillas. **Las listas son excelentes para usar cuando desea trabajar con muchos valores relacionados.**

Los Tuplas no son elementos cambiables ni modificables dentro del codigo una vez creado.

Se puede usar el metodo list() y tuple() para convertirlo

# Tipos de Operadores

| + | Suma | - | Resta |
| --- | --- | --- | --- |
| * | Multiplicación  | / | División |
| // | División sin decimal | % | División absoluta, “1 o 2” |
| < | Menor que | > | Mayor que |
| ≤ | Menor o igual que | ≥ | Mayor o igual que |
| == | Igualdad | ≠ | Diferente |

# Condicionales

Son uno de los componentes mas ********utilizada******** y es una instrucción, siendo un predicado cual valida su veracidad , estableciendo cuadno se ejecuta o no un código determinado. Esta tiene 3 componentes:

- if: si algo se cumple

	- Inicio

- elif: si no se cumplió algo y se comple otra cosa

	- Es el unico que puede aparecer muchas veces

- else: si no se cumple nada de lo anterior 

	- Final

Para hacer un if es hacer una comparación (menor que, mayor que, igual que...)



# Formateo de string
> Este es un tema algo mas para adelante pero se ordena mas aqui 

```python

#Con **MARCAS**

%s = para poner dentro de un strin 
b = input("")
c = input("")
d = input("")
a = " aha %s %s, como que %s" % (b, c, d)


"""
a = "el modelo %s es %s"
a = a % (b,c,d)

"""
Nombre = "Juan"
Prof = "Abogado"

a = "La Hilera es de %(Nombre1)s, y es un %(Prof12)s, por lo cual confia en el"

a = a % {
        "Nombre1" : nombre,
        "Prof12" : Prof
    }

#%f es un float
"""
% + <decimales que quieres [.0 → 0 a la izquierda]> + f
"""

para usar %s como % s 
\%\s

b = "Juan"
c = "Pérez"
d = "Deudas"
f = 10.687861786871
a = f"El nombre de la persona es {b} y sus apellido es {c}"

#para limitar los decimales
z = f"{b}{c} tiene una {d} de {f: .1}" #.1 slo un decimal

a = f"El nombre de la persona es {b}".format(salario)
```


---

# s
![[Python]]

