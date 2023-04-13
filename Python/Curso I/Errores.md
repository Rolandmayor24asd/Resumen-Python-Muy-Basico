
---
Tema: Evitar errores
Curso: I
Orden: 7
Clases: 7
---

# Evitar errores

Para evitar que se caiga el codigo por un error mediante una jerarquia de excepciones, estas jerarquias son usados en el codigo `try` y el codigo `except`

![Untitled](Curso%20I/Funciones/Untitled.png)

Se debe reconocer donde puede suceder el error! 

Estructura:

```python
try:
	codigo que validar
except + <nombre de una exepcion que quiero validar> + :
#lo de la tablita la exepcion
	lo que quieres que pase si falla 

finally: #siempre al final y siempre ocurre 
	

#para levantar un error de forma artificial
raise + error correspodiente 

```
> Los errores correspondientes son los de la foto o puedes buscarlos en [esta pagina](https://docs.python.org/es/3/tutorial/errors.html)

---

![[Python]]