---
Tema: Funciones de python y propias
Curso: I
Orden: 8
---


# Funciones

Seccion de codigo que definimos dentro de un codigo 

> Variable llenada de de codigo que no interfiere con el cupero principal

## Importanción

Tambien hay otras conocidas como librerias que debes importar pero esta seran vistas en [[Funciones exteriores]]

## Creación

 Y las funciones que crea el programador tiene la siguiente sintaxis de ```def + nombre + (parametro)``` como en el siguiente cuadro:
 
```python
#creación de la función
def + *nombre de la función +* (<parametros>):
	Codigo que quieres que siempre quieres que copie

#llamado de la función
*nombre de la función(parametros de la función solicite)

#Se puede definir funciones dentro de funciones pero solo dentro de su propia funcion* 
```

> Ninguna función va usar input definiendo antes [Tampoco para solo usar locals pero por temas del porpio Python ]) y print para los trabajos de Python #1
> 

## Parametros en las funciones

Como “quitar los imputs”,  puedes definir la información afuera y deepues hacer que a la vez que cree su busqueda en local sea a global con el comando `global + variable`.

```python
def ejemplo(variable1,variable2, ... <tanto como quieres>): #firma de una función
	variable1 = float(variable1)
	variable2 = float(variable2)
	print("el resultado es", variable1 + variable2 2)

ejemplo(<lo que pones para variables que pusistes>)
 
```

> La función funciona como un encalupsado, provocando que lo de afuera no le afecte (variables o ect debe estar dentro de la misma) y todo lo que se defina adentro no afecta a fuera de el mismo.

### Parametros sin determinar
> Para poner un parametro para poner muchas cosas se debe usar  `*`, este creara una dupla, por lo cual puedes meter una lista, y esta sera aceptada, para sacarle provecho debemos de usar los ciclos

```python

def print(*args)
				#*args = La variable puede obtener muchas siendo una lista
calcuradora1(1, 25,36,\ #obligatorios 
 operacion="suma", imprimir=True, retornar= False) #opcionales
				
```


#### Trabajar las listas con los ciclos

El interprete entiende el `for` + lista como si pasa cada vez que pasa algo con uno de la lista, por lo cual esto hace que puedas buscar cosas dentro de la misma

Por lo cual puedes crear funciones que aprovechen la lista:
```python

def ejemplo (*args):
	a = 0
	for args in args
		 a += args
	return a


```


## Return

Toda función devuelve `none` sin importar nada pero su estructura es excepto por [[Temas Varios#Generadores|aqui]]

```python
return + variable/<numero o algo>
#devuelve en la misma linea por lo cual 

def ejemplo(variable1,variable2, ... <tanto como quieres>): #firma de una función
	variable1 = float(variable1)
	variable2 = float(variable2)
	resultado = variable1 + variable2
	return resultado

variable = ejemplo(<lo que pones para variables que pusistes>)
print(variable)
```

Todo lo que esta despues de retorno no hace que se ejecute lo demas del codigo de la función, osea es como un exit para devolver los valores.
> El retorno es la unica manera de devolver un valor definido dentro de la misma función

### No print dentro de las funciones

Usando el `return` como en el ejemplo de arriba

```python
return + variable/<numero o algo>
#devuelve en la misma linea por lo cual 

def ejemplo(variable1,variable2, ... <tanto como quieres>):
	variable1 = float(variable1)
	variable2 = float(variable2)
	resultado = variable1 + variable2
	return resultado 

variable = ejemplo(<lo que pones para variables que pusistes>)
print(variable)
```

>Esto para usar las variables y el return manteniendo una estructura, y cuando tienes mas de una pagina algunas de ellas solo es para escribir funciones que seran llamadas.

### Dejar algo vacio

 Para salatarse es `pass` para evirtar problemas o crear pruebas, muy util con comandos while donde defines un menu (ejemplo) y  ya sabes los numeros pero aun no su estructura se pone ```pass```, puede usarse en funciones, ciclos, ect.
 
 ```python
 def a (primero,segundo):
	 pass



 ```

### Ejemplo de una función 

```python
lista = ("banano", "fresa", "kiwi", "melon", "papaya")

def verificar(lista, fruta):
    se_encuentra = fruta in lista
    cantidad = 0 
    if se_encuentra == True:
        cantidad = lista.count(fruta)
    return se_encuentra, cantidad

nombre_fruta = input("ingrese")

encontrada, cantidad = verificar(lista, nombre_fruta)
if encontrada == True:
    print("SE ENCONTRO!!!", nombre_fruta, "un total de", cantidad)
else:
    print("Como que no esta jajaja")
```

```python
def ejemplo(variable1,variable2):
	variable1 = float(variable1)
	variable2 = float(variable2)
	resultado = variable1 + variable2
	return resultado

b = caso1 = ejemplo(1,1)
a = caso2 = ejemplo(12.05,12)

print(a, "y", b, "suman un total" a + b)
```


Mas tipo de funciones que puedes crear es lamba escrita aquí [[Temas Varios#Funciones lamba|Funciones lamba]]




## Definidas
[Documentación de Python - 3.11.3](https://docs.python.org/es/3/library/functions.html)

Ya hay funciones definida en el propio Python por medio del interprete como por ejemplo

```python
#imprimir
print(variable, end="como termina",\
	 sep="como quieres que divida la ','"\
		file="aun no")

#crea algo en lista
list(variable)

Funciones = Listas 

#agregar algo al final de la lista
.append()

#elimina todos los elementos a una lista
.clear()#vacio siempre

#Borrar un solo elemento
.remove()
	#si tiene dos veces la misma palabra solo borra la primera de ellas
#solo en uno en uno
    while "melon" in lista:
        lista.remove("melon")

#busca la primera ucurrencia y el indice cual esta
.index()

#devolver el elemento borrando y poniendo la primera  
.pop()
	#recibe indice para saber cual es 
	#si pones un parentesis vacio es el ultimo de la lista

#Ordena la lista de menor a mayor
.sort()
	.sort(reverse=Tue) #lo vuelve de mayor a menor
	
#da vuelta a los elementos
.reverse

Funciones = diccionarios
#para ver los terminos del diccionario
.keys 

#Para buscar la variable
.get 

**#enumerar
enumerate**

#cambiar cualquier intercambio

#par acambiar indice a con indice x

lista = [leche , jugo ]
temporal = lista [0]
lista [0] = lista [1]
lista [1] = temporal

lista [0], lista [1] = lista [1], lista [0]
```

[Ver mas aqui](https://docs.python.org/es/3/library/functions.html)

---

![[Python]]