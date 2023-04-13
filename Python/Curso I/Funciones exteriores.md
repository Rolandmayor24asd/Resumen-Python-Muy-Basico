
---
Tema: Funciones importadas
Curso: I
Orden: 9
---

# Modulos de Python

Que define para no ocupar llenar la memoria y no ocupa cargar todo lo de python evitando tener variables, funciones y documentación. Tambien para evitar usar solo un documento 

# Funciones Import
En python hay funciones que aunque vienen dentro del lenguaje se deben atraer como por ejemplo 

```python
import statistics 
	max = numero maximo de una lista 
	min = numero minimo de una lista
	
```



Puedes ver la documentación completa aqui → [The Python Standard Library — Python 3.11.3 documentation](https://docs.python.org/3/library/index.html) pero aqui escrbire algunos ejemplos


-   `math`: Este módulo proporciona acceso a las funciones matemáticas definidas por el estándar C. Por ejemplo:

```python
import math
x = math.sqrt(4)
print(x) # 2.0
```

-   `random`: Este módulo implementa generadores de números pseudoaleatorios para varias distribuciones. Por ejemplo:

```python
import random
x = random.randint(1, 10)
print(x) # Imprime un número aleatorio entre 1 y 10
```

-   `datetime`: El módulo datetime suministra clases para manipular fechas y horas. Por ejemplo:

```python
from datetime import datetime
now = datetime.now()
print(now) # Imprime la fecha y hora actual


from #desde dentro de python
from datetime import <Lo que deseas importar; timedelta|tzinfo|date...>

```

- Timedelta
	- Modificar hora
- Tzinfo
	- Hora horaria
- Date
	- Para poner dia-mes-año


-   `os`: Este módulo proporciona una forma portátil de utilizar la funcionalidad dependiente del sistema operativo. Por ejemplo:

```python
import os
os.mkdir('test') # Crea un directorio llamado 'test'
```

-   `sys`: Este módulo proporciona acceso a algunas variables utilizadas o mantenidas por el intérprete y a funciones que interactúan fuertemente con el intérprete. Por ejemplo:

```python
import sys
print(sys.version) # Imprime la versión de Python en uso
```

-   `re`: Este módulo proporciona operaciones de coincidencia de expresiones regulares. Por ejemplo:

```python
import re
x = re.search(r'\d+', 'abc123def')
print(x.group()) # Imprime '123'
```






# División

Primero crearemos un folder .Crearemos modulos para contener solo funciones, variables ext…

> Solo definiciones


Para atraerlos debo de hacer lo de atraer igual modulos con importación relativa

```python
from <Nombre del doc donde esta las funciones o variables> import <funciones|variables>
import <pagina> #Con todos las funciones 

```




---

![[Python]]



