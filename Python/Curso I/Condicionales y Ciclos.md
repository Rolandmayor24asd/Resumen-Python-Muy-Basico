---
Tema: Condicionales y Ciclos
Curso: I
Orden: 5
Clases: 5
---

# Condicionales

---

Son uno de los componentes mas ********utilizada******** y es una instrucción, siendo un predicado cual valida su veracidad , estableciendo cuadno se ejecuta o no un código determinado. Esta tiene 3 componentes:

- if: **si algo se cumple**
	- Inicio


- elif: **si no se cumplió algo y se comple otra cosa**
	- Es el unico que puede aparecer muchas veces

- else: **si no se cumple nada de lo anterior** 
	- Final


Para hacer un if es hacer una comparación (menor que, mayor que…)

# Validación (No tan completa pero funcional)

`.is` (Msa variables pero se ven en visual):

- `.isdigit`
    - Para saber si es un numero positivo

Formula: Condicional + variable + .is + == + True/False + :

### Expresiones regulares (no dada en este topico)

# Operador condicional

Estos ponen la condiciones en una union o intersección

- Y condicional “and”
    - Los dos se convierte en un unico condicional (ambos tienen que ser verdadero)
- O condicional “or”
    - Unifica dos codiciones para ver si algun factor se cumple

Siempre ejecuta primero los “and” y depues ejecuta los “or”, para obligar el orden usar “()”

## Tablas de la verdad

En las tablas “AND”

![Untitled](Curso%20I/Continuación/Untitled.png)

Si el dia de la semana es LUNES “A” y la hora del dia es de NOCHE “B” es vd+vd= vd

En las tables “OR”

![Untitled](Untitled%201.png)

---

# Ciclos

Los bucles se utiliza para crear repeticiones de cierto codigo 

- While
    - No sé cuantas veces se repite el codigo
        - Solo comparación
            - De la manera
                
                ```python
                while a == a:
                    #Si se cumple la condición se crea entra y crea
                
                ```
                
- For
    - El mas utilizado
    - Yo se cuantas veces se repite el codigo
        - Con `range`
            - De la forma
                
                ```python
                x = range (inicio, final)
                
                x = range (inicio, final, los saltos)
                ```
                
    - Condición de parada:
    

> Bucles infinitos; cuando falta la condición de parada y no se busca, excepto por algunas cualidades como en videojuegos (como revisar algo)
> 
## For


Para la esturcutra de los “for” fuera:

```python
for "x" in range (inicio, final) :
    print (x)
```

```python
for "x" in range (inicio, final, cantidad de saltos) :
    print (x)
```

### Forzar finalizar

```python
import sys
sys.exit("Datos invalidos, vuevle a intentarlo") #Saca y hace un print
```

Crear linea/cuadro 

```python
for horizontal in range(0, 10):
    puntos = " "
    for horizontal in range(0, 10):
            puntos += "* "
    print(puntos)

for horizontal in range(0, 10):
    puntos = " "
    for horizontal in range(0, 4):
        puntos += "* "
    for horizontal in range(0, 3):
        puntos += "* "
    for horizontal in range(0, 4):
        puntos += "* "
print(puntos)
```


Los bucles se utiliza para crear repeticiones de cierto codigo 

## While
- No sé cuantas veces se repite el codigo
    - Solo comparación
        - De la manera
    
```python
     while a <comparación> b:
	    cuerpo del ciclo     
```
            


---

![[Python]]