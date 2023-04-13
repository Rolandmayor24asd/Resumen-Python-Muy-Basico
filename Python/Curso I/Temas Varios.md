
---
Tema: Temas varios
Curso: I
Orden: 11

---

# Namesspace

Como organisar programas

> main.py 

|———————-funciones_matematicas

|——————geometria.py

|——————algebra.py

|——————derivación.py

|———————-funciones_trignometrica

|——————logica.py

|——————inversa.py

Para crear simpre se inicia en **main.py** y crear el ambiente

# Funciones lamba

Cuando una función no tiene mucho código (1 sola linea)

```python
def cuadrado(num):
    return num**2
"""
↑↓ Lo de arriba y abajo es igual 
"""
lambda + <lo que entra> + : + <que quiero que regrese> + <datos>
#Un solo uso
lambda num : num ** 2 (<datos>)
#Muchos usos
variable = lambda num : num ** 2

#Llamar la desechable
resultado = (lambda num:num ** 2) (2)

#Llamar la anonima (**Solo con el interprete**)!!!!!!!!!
_(4)

#Llamar la función
resultado = variable (2)

#definimos
def ejectuar_funciones(funcion, variable1, variable2 = None, Variable3 = None):
    return funcion(*args)

imprimir = ejecutar_funciones(variable, 2)
print(imprimir)

```

# Funciones filtro

Filtren los elementos iterables mediante un criterio

```python
def devolver_pares(lista):
    lista_pares = []
    for numero in lista :
        if numero % 2 == 0:
            lista_pares.append(numero)
    return lista_pares

lista = [1,2,3,4,5,6,7,8,9,0]

resula = filter(devolver_pares, lista)
```

# Acciones inline

Sustituir una lista por una lista pasada en cierto parametro en cada parametro

```python
lista = [1,2,3,4,5,6,7,8,9,0]

# for index,valor in enumerate(lista):
#     lista[index] = pow(valor,2)

lista = [ pow(valor,2) for valor in lista ] #Ya saber el itenario

print(lista)
#Si es mucho mucho la info puede ser malo 
```

# Decoradores

Es para ampliar cada una de las ufnciones

```python
def flotantes(funcion)
    def encapsula(*args, **kwards)
        for valor in args:
            if type(valor) != float:
						    print("Almenos uno de los valores no es compatible")
                return 

        funcion(*args, **kwards)
    return encapsula

@ flotante
def suma(v1,v2)
    return v1 + v2

suma(1,"12")
```

# Generadores

Ir creando una lista uno a uno borrando lo pasado, muy util para los archivos

 

```python
yield (lo que es un generador)
 #Solo funciona una vez ya que ponje uno borra el anterior, pone otro ect

def generar_impares(n):
    for contador in range(0,n):
        impar = 2 *contador +1
        yield impar #Guarda solo una variable y su posición 

generador = generar_impares(30)
for x in generador:
    print(x,end=".")
```

---

![[Python]]