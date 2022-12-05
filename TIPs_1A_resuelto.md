
# Bienvenidos a las TIP's. 
Recuerda que esto es una herramienta para practicar como seria una entrevista real! Pero en un ambiente seguro :blush:<br>
Bajo ningun punto de vista queremos su compañer@ pase un mal momento! Simplemente guialo a traves de las preguntas<br>
<sub>No le des las respuestas facilmente, pero sueltale pistas si l@ ves un poco perdido@ :wink:

<br>
  
### **1) ¿Qué tipos nativos de estructuras de datos de Python conoces? ¿Cuáles son inmutables?**

__Respuesta Esperada__:   _Las estructuras de datos nativas en Python son las listas, los diccionarios, las tuplas y los sets, estos últimos dos son inmutables (no puedes cambiar su contenido una vez declarados)._

### **2)¿Qué es una variable categórica en Pandas?**

__Respuesta Esperada__:   _Las VARIABLES CATEGÓRICAS son un tipo de dato que maneja nativamente pandas (type=category). Una variable categórica toma solo una categoría fija(generalmente un número fijo) de valores. Algunos ejemplos de variables categóricas son género, grupo sanguíneo, idioma, etc. Un contraste principal con estas variables es que no se pueden realizar operaciones matemáticas con estas variables._

### **3) ¿Qué tipo de filtros pueden implementarse en POWER BI?**

__Respuesta Esperada__:   

  
  
  _Pueden implementarse 3 tipos de filtros:_
  - Filtros a nivel visualización: Filtra tanto datos como medidas calculadas, limitando la cantidad de información que puede verse en una visualización determinada.

  - Filtros a nivel página: Filtra la info en todas las visualizaciones de una página específica del reporte.

  - Filtros a nivel reporte: se aplican a todas las páginas y visualizaciones en simultáneo.

<br>
<br>
  

## Suponga que tiene las tablas *SALAS* y *PELICULAS* compuestas de la siguiente forma.

### SALAS                     

| `PK` | Codigo | int |
|--------|--------|:--------:|
|  | Nombre | nvarchar(100) |
| `FK1`  | Pelicula  | int |
  

### PELICULAS
  
| `PK` | Codigo | int |
|--------|:--------|:--------:|
|  | Nombre | nvarchar(100) |
|  | CalificacionEdad  | int |
  
Note que existe una relacion entre *`FK1` - Pelicula* de la tabla SALAS y *`PK`-Codigo* de la tabla PELICULAS
  
<br>

## Con dichas tablas construya las siguientes queries:
### **4) Seleccione todas las salas que no estan proyectando ninguna pelicula** </p>

<br>
  
__Respuesta Esperada__:
```sql
SELECT * 
FROM SALAS 
WHERE Pelicula IS NULL
```
<br>

### **5) Actualice las peliculas que no han sido calificadas como no recomendables para menores de 16 años.**
<br>
  
__Respuesta Esperada__:
```sql
UPDATE PELICULAS SET  CalificacionEdad=16
WHERE CalificacionEdad IS NULL
```

  
### **6) Seleccione los nombres de las pelıculas que no se proyectan en ninguna sala.**
  
<br>
  
__Respuesta Esperada__:   
<sub>Con JOIN<sub>
```sql
SELECT PELICULAS.Nombre
FROM SALAS RIGHT JOIN PELICULAS
ON SALAS.Pelicula = PELICULAS.
```
<br>
  
<sub>Con Subconsulta<sub>


```sql
SELECT Nombre 
FROM PELICULAS
WHERE Codigo NOT IN (
SELECT Pelicula FROM SALAS
WHERE Pelicula IS NOT NULL
)
```

