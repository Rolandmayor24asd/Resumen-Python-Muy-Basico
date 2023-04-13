---
Tema: Colección de Datos 
Curso: I
Orden: 6
Clases: 6
---

# LEN

Igual a forma de saber la cantidad que tiene algo. que relamente es una función que se ve [[Funciones|aqui]] ya traida por el propio Python

# Colecciones de datos

Son unicas y 4 (en este curso 3), colección de datos puede ser un conjunto de elemento de otra colección o las mismas (finitos de manera dinamica, pero valor infinito)

- Tuplas (tuples)
    - No permite cambios de agregar y quitar
- Listas (list)
- Diccionarios (dict)
	- Termino con pareja

## Tuplas “()”

Para crear una tuplas es con parentesís, y dentro de ellos (sin importar que sea; numero, stringer, flotante…) , se separan con comas,.

```python
variable = (elementos que queremos agregar a la tuplas) #()→ representa las tuplas 
```

Para acceder a los elementos de tuplas, esto mediante el Índice ( del 0 al infinito)

```python
dias_semanas = ("Lunes","Martes","Miercoles","Jueves","Viernes","Sabado","Domingo")
# numeración       0        1         2          3        4        5          6
# numeración      -7       -6        -5         -4       -3       -2         -1

print(dias_semanas[numero del indice que quiero ])
```

Para saber el tamaño de una tupla es: 

```python
len(variable)
variable = len(variables con duda)
#tambien puede ser usado para saber cuantos caracteres tiene cosas (strings...)
```

Estas apenas son definidas no se pueden cambiar, por lo cual normalmente se usa algo que no ocupa cambios (dias de la semana, meses del año, todo lo constante)

Las tuplas pueden tener valores repertidos 

## Listas "[]"

Similar a las tuplas, la diferencia es que se puede; agregar, quitar… osea totalmente modificable, 

```python
variable = [elementos que queremos agregar a las listas] #[]→ representa las listas
```

Las listas tiene el mismo indice 

```python
nombres = [                                                                       ]
# numeración       0        1         2          3        4        5          6
# numeración      -7       -6        -5         -4       -3       -2         -1

print(nombres[numero del indice que quiero ])
```

Para agregar en la lista se usa

```python
<variable donde esta la lista> + . + append + <variable que quieres agregarz>
nombres.append("Eduardo")
```

## Diccionario "{}"

Puede iniciar vacio o con inforamción, 

```python
diccionario = { 
    "ptermino" : "valor del string", #nivel 1
		"x" : "y",
		"direccion" : ("A", "C", "D" )
}

```

Para sacar la info 

```python
print( diccionario["termino"])
```

Para agregar/modificar variables que existen 

```python
diccionario["terminario"] = "lo que significa"
```

Se puede hacer una jerarquia 

```python
diccionario = { 
    "ptermino" : "valor del string", #nivel 1
		"x"             : "y",
		"punto": {
				"a" : "z"
				"b" : "c"
				"Kns" : {
						"aja" : "wow"
						"numersodj" : 1
						}
		}
		"direccion" : ("A", "C", "D" )
}

```


---

# Index

Tiene un pequeño problema 

```python
Lista = ["A", "E", "I"]
print( lista.index(<variable que quiero>))
#debe ser exacto  y para en la primera variable igual
```

# in

```python

if numero/palabra in lista: #not antes del in para negación
	print("El numero ya esta en la lista")
else:
	list.append(numero)
```

```python
if lista.count(numero) == 0:
    lista.append(numero)
else:
	print("El numero ya esta en la lista")
```

---

![[Python]]