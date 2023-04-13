
---
Tema: Captura de paginas
Curso: I
Orden: 10

---


# Dos formas de guardar archivos

- Texto plano
    - Cuando como humano puedes leerlo/ trabajar/revisar
- Archivos en binario
    - No tan leibles

La computador guarda es ASCCI, UTF8…

1. ASCCI
    1. 8 bits posicciones en 0-1
2. UTF8 
    1. 16-32 bits

Pasos

> 1. Abrir
> 2. Editar
> 3. Cerrar

# Abrir

Primero debes ubicar el archivo;

- Relativa
    - Llegar desde el ejecutador del codigo
	    - Solo con el nombre
- Absolutas
    - Ruta absoluta donde esta ubicado en el dispositivo
	    - Ruta completa

```python
ruta = "archivo.txt" #ruta relativa
aricho = open(ruta, mode='r' + <encoding="utf-8">) # El modo "r"
```

- Modos que se puede abrir los archivos:
		- r → archivo para lectura
		- w → sobreescribir 
		- x → crear archivo
		- a → abrir para agregar información al final del archivo 
		- b → abrir modo binario
		- t → modo texto
		- "+" → Leer y escribir
> De manera predetermindada es rt [Lectra de archivo de texto]
> Tambien puede ser combinado

# Leer

Despues de abrir el archivo y decidir su modo lectura se debe 

```python
Archivo = archivo.read() #Pone todo el archivo en la variable
Archivo = archivo.readline() #Solo lee una linea por linea
#	Normalmente para el readline se ocupa un while

```

# Escribir y edita

Dos modos, el a y w, el w siempre sobreescribe y el a crea nuevo o agrega al final

```python

Editar = open(ruta, "a+", encoding="UTF-8")
Editar.write('Texto que quieres agregar')
Editar.close()

```

While

Abriri y cerrar los archivos

```python
#igual que anes
a = "pie.move"
acopia = "aosefj.ifa"

with open(a, "r") as origi:
	with open(acopia, "r") as copia:
		Cuerpo 

```

---

![[Python]]
