
# Bienvenidos a las TIP's. 
Recuerda que esto es una herramienta para practicar como seria una entrevista real! Pero en un ambiente seguro :blush:<br>
Bajo ningun punto de vista queremos su compañer@ pase un mal momento! Simplemente guialo a traves de las preguntas<br>
<sub>No le des las respuestas facilmente, pero sueltale pistas si l@ ves un poco perdido@ :wink:

<br>
  
### **1) ¿Cuál es la principal diferencia entre listas y sets? Nombre dos operaciones posibles con sets**

__Respuesta Esperada__:   _Tantos los sets como las listas, son de las 4 estructuras nativas de Python. Los sets, a diferencia de las listas, son inmutables, no admiten duplicados ni ordenamiento. Los sets permiten hacer operaciones como intersection, union, difference y symmetric difference_

### **2)¿Qué enuncia el teorema CAP?**  
<br>

__Respuesta Esperada__:   

_El teorema CAP, o conjetura de Brewer, enuncia que ningún sistema de almacenamiento de datos puede garantizar en forma simultánea:_
  - _Consistency_
  - _Availability_
  - _Partitioning tolerance_

### **3) ¿Cuál es la diferencia entre medida calculada, columna calculada y tabla calculada?**

__Respuesta Esperada__:   

- _Columna Calculada:_
  - _Se agregan a tablas existentes mediante fórmulas DAX sobre columnas existentes_
  - _Define y almacena valores en una columna nueva sin hacer query a la fuente de datos_
- _Tabla calculada:_
  - _Creada mediante fórmula DAX para definir todos sus valores_
_Puede crearse tanto en Vista Reporte como en Vista Data_
- _Medidas:_
  - _Se realizan a través de la query_

<br>
  
<hr>

## Suponga que tiene las tablas *Albumes* y *Canciones* compuestas de la siguiente forma.

### Albumes                     

| `PK` | Codigo | int |
|--------|--------|:--------:|
|  | Nombre | nvarchar(100) |
|  | Artista  | nvarchar(100) |
  

### Canciones
  
| `PK` | Codigo | int |
|--------|:--------|:--------:|
| `FK1`| Codigo_album | int
|  | Nombre | nvarchar(100) |
|  | CalificacionEdad  | int |
|  | Duracion  | int |
  
Note que existe una relacion entre *`FK1` - Codigo_album* de la tabla Canciones y *`PK`-Codigo* de la tabla Albumes
  
<br>

## Con dichas tablas construya las siguientes queries:
### **4) Seleccione todos los artistas que tengan al menos 2 álbumes** </p>

<br>
  
__Respuesta Esperada__:
```sql
SELECT Artista, COUNT(Codigo) as Cantidad_albumes
FROM Albumes 
GROUP BY Artista
HAVING COUNT(Codigo) <= 2;
```
<br>

### **5) Seleccione los valores únicos de artistas de la tabla álbumes y ordenelos de la Z a la A.**
  
<br>
  
__Respuesta Esperada__:   

```sql
SELECT DISTINCT Artista
FROM Albumes 
ORDER BY Artista DESC;
```
<br>


