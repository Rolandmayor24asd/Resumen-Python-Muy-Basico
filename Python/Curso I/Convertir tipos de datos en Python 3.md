---
Tema: Bases del lenguaje 
Curso: I
Orden: 4
Clases: 4 
---

Los tipos de datos se utilizan para clasificar un tipo específico de datos, deberá aplicar conversiones de valores entre tipos para manipular los valores de forma diferente.

Inciamos con lso tipos de datos a convertir, estos son; números, cadenas, tuplas y listas.

## **Numeros**

En Python hay dos tipos de datos numéricos; números enteros y de punto flotante (flotantes)

La conversión fuera de numero entero → flotante o viceversa

> Entero → Flotante

```python
float(x) #lo convierte en x.0 (poniendolo en el print)
print(float(x))
```

> Flotantes → Enteros 

```python
int(x) #le quita los desimales "SIN REDONDEAR" 
```

## **Cadenas y numeros**

La secuencia de caracteres (letras, números, símbolos), y se convierte normalmente entre cadenas y números cuando es tomado datos generados por el usuario, o si ocupas mezclar ambos 

> Numero → Cadena (stringer)

```python
str(12) #en la terminal convierte 12 en "12" en el  output
```

Usado para poder usar el numero en el texto sin dar error, podemos realizar una prueba para asegurarnos de que esté bien, realizando una concatenación con una cadena.

> Cadena (stringer) → Numero

Este puede ser utilizado para restar dos variables cuando las variables estan usando “120” como cadena a la vez de 120. En estos casos usamos int (para volverlo entero) o float(para volverlo flotante) teniendo como ejemplo

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

Se puede usar el metodo list() y tuple() para convertirlo

## **Booleano (Boolean)**

Es el True, False, 0, 1 (el on y off de toda la vida)

```python
bool() #su forma de representaicón en Python para cambiar 
```

## **Tuplas y Listas**

Las listas es una secuencia ordenada de elementos mutables contenidas entre corchetes “[]” y la tupla es la secuancia oredenada de elementos inmutables contenida entre paréntesis “()” mas especifico

Las listas son elementos cambiable en secuencia ordenada, estos son definidos entre comillas. **Las listas son excelentes para usar cuando desea trabajar con muchos valores relacionados.**

Los Tuplas no son elementos cambiables ni modificables dentro del codigo una vez creado.
[[Colecciones de datos#Colecciones de datos|Conectado con esto]]]

![[Python]]