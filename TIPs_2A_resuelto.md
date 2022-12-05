


# Bienvenidos a las TIP's. 
Recuerda que esto es una herramienta para practicar como seria una entrevista real! Pero en un ambiente seguro :blush:<br>
Bajo ningun punto de vista queremos su compañer@ pase un mal momento! Simplemente guialo a traves de las preguntas<br>
<sub>No le des las respuestas facilmente, pero sueltale pistas si l@ ves un poco perdido@ :wink:

<br>
  
### **1) Qué son las formas normales en bases de datos?**

__Respuesta Esperada__:   _Son una serie de normas que se aplican a las tablas de datos para cumplir con la propiedad deseable de no redundancia. Son 5 formas normales y en general, se considera que una base de datos está correctamente normalizada si llega por lo menos a la tercera forma normal (3F)_

### **2) Explique que es una función de agregación y mencione al menos 5 de las más comunes**

__Respuesta Esperada__:   _Las funciones de agregación realizan análisis estadísticos sobre número (o fechas en algunos casos). Algunas de las funciones de agregación más comunes son: Count, AVG, Max, Min, STDDEV, Varianc_

### **3) El entrevistador es “Tech Lead *Data Analytics*” de Mercadolibre: Tienes alguna idea o sugerencia para que podamos mejorar?**

__Respuesta Esperada__:   _No hay respuesta correcta!_

<br>
  <br>
  
## Ejercicio practico python: Diccionario Jeringozo
  
Cree un programa que tome una lista de palabras en minusculas y devuelva un diccionario que
contenga la palabra original como llave y la palabra en jeringozo como valor.

  El _jeringozo_ es una criplolalia (manera de codificar el habla) que suelen
utilizar los niños para jugar en los países hispanohablantes. Consiste en agregar
después de cada sílaba una "p" y se repite la vocal.

   
`Input`: lista = ['banana', 'manzana', 'mandarina']
  
`Output`: {'banana': 'bapanapanapa', 'manzana': 'mapanzapanapa', 'mandarina': 'mapandaparipinapa'}

__Respuesta Esperada__: 
  
```
lista = ['banana', 'manzana', 'mandarina']
cadena= ",".join(lista) 
capadepenapa = ''


for c in cadena:
    capadepenapa += c
    if c in "aeiou":
        capadepenapa += "p" + c 

dicjeringozo = dict(zip(cadena.split(","), capadepenapa.split(","))) 
print(dicjeringozo)
``` 

