<h1>TIPS: Technical Interview Preparation</h1>
<h2>Grupo A --&gt; Segundo Set de Tips con Respuestas</h2>
<h2>NO MOSTRAR A SUS PAREJAS DE TIPS!</h2>
<h3>1)  Respuesta:</h3>
<p>Un JOIN interno en SQL devuelve solo los registros que tienen coincidencias en ambas tablas, mientras que un JOIN externo devuelve todos los registros de una tabla y los registros coincidentes de otra tabla. </p>
<h3>2)  Respuesta:</h3>
<p>Lista: mutable, velocidad inferior y utilización de corchetes

Tupla: inmutable, velocidad superior y utilización de paréntesis </p>
<h3>3)  Respuesta:</h3>
<p>El nivel en los lenguajes de programación se refiere a qué tan parecido es al código que leen los procesadores, mientras más bajo sea el nivel, más similar al código que leen los procesadores y más rápido podrá ser procesado una vez compilado, pero como contraparte mucho más complejo será escribir dicho código, mientras mayor sea el nivel, más fácil es expresarlo para las personas, más natural al humano, pero es costoso de compilar y se procesan menos eficientemente. Python se considera un lenguaje de alto nivel, con una sintaxis muy simplificada que facilita la creación de código. Es un lenguaje interpretado, no necesita ser compilado, sino que el intérprete de Python va leyendo e interpretando el código una vez que es ejecutado. </p>
<h3>4)  Respuesta:</h3>
<p>Pueden implementarse 3 tipos de filtros:</p>
<p>Filtros a nivel visualización: filtra tanto datos como medidas calculadas, limitando la cantidad de información que puede verse en una visualización determinada</p>
<p>Filtros a nivel página: filtra la info en todas las visualizaciones de una página específica del reporte</p>
<p>Filtros a nivel reporte: se aplican a todas las páginas y visualizaciones en simultáneo</p>
<h3>5)  Respuesta:</h3>
<p>La probabilidad de que la persona seleccionada sea del grupo A es simplemente el porcentaje de personas del grupo A en la muestra, que es del 60%. Por lo tanto, la probabilidad de que la persona seleccionada sea A es del 60%. </p>

<h3>6)  Respuesta:</h3>
<p>La distribución normal es una distribución de probabilidad continua que se utiliza para modelar muchos fenómenos naturales y sociales. La distribución normal se caracteriza por una curva en forma de campana y se utiliza para describir variables que tienen una distribución simétrica.</p>

<br>

# Ejercicio practico SQL
### Suponga que tiene las tablas *SALAS* y *PELICULAS* compuestas de la siguiente forma.

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
### **a) Seleccione los valores unicos de calificaciones de edad que existen.**
<br>
  
__Solucion propuesta__:
```sql
SELECT DISTINCT CalificacionEdad 
FROM PELICULAS
```


### **b) Se ha agregado una nueva pelicula llamada "Hola, Mundo" para mayores de 8 años. Actualice la tabla correspondiente**
<br>
  
__Solucion propuesta__:
```sql
INSERT INTO PELICULAS (Nombre, CalificacionEdad)
VALUES ("Hola, Mundo", 8)
```

  
### **c) Seleccione todas las salas, y si se proyecta alguna pelicula en la sala, selecciones tambien la informacion de la pelicula proyectada**
  
<br>
  
__Solucion propuesta__:   

```sql
SELECT *
FROM SALAS LEFT JOIN PELICULAS
ON SALAS.Pelicula = PELICULAS.Codigo
```
<br>
  
