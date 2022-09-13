# Henry - TIPS Grupo A

## **Cuestionario**:
### **1) Describa la diferencia entre claves primarias y foráneas en una base de datos SQL.**  
__Respuesta Esperada__:   _Las claves primarias (o primary key) es el campo, o conjunto de campos, que nos permite identificar de forma única un registro. Las claves foráneas (o foreign key) es un campo, o conjunto de campos, que nos permite relacionar un registro de una tabla con otro, generalmente en una tabla distinta._ 

### **2) Comentar la diferencia entre las variables locales y las variables globales.**
__Respuesta Esperada__:   _Las VARIABLES GLOBALES son las declaradas fuera de una función. Todas las funciones del código pueden acceder a dicha variables. En cambio, las VARIABLES LOCALES son aquellas creadas dentro de las funciones. Intentar acceder a ellas fuera de la función devolverá una falla del sistema._ 

### **3) En un sobre hay 20 papeles, 8 poseen un dibujo de un coche, las restantes son blancas. Hallar la probabilidad de extraer al menos un papel con el dibujo de un coche si:**  
**a)** se saca solo 1 papel.  
__Respuesta Esperada__:   _8 casos favorables sobre 20 posibles. RTA= 2/5 O 0.4_   
**b)** se sacan 2 papeles.    
__Respuesta Esperada__:   _La probabilidad de que al sacar 2 papeles al menos tenga un coche menos la probabilidad de que al sacar 2 papeles las dos sean blancas. Es decir:_    
Probabilidad = 1 - ((12/20) . (11/19))   
Probabilidad = 62/95  o 0.6526....


## Suponga tiene la tabla ARTICULOS compuesta de la siguiente forma:

| IDArticulo | PRECIO | Proveedor |
|--------|--------|----|
| valor | valor | valor |
|valor  | valor  | valor |


### **4) Cree una consulta SQL que obtenga los datos de la tabla ARTICULOS atículos cuyo PRECIO esté entre los 60 y los 120 USD (ambas cantidades incluidas) .**
__Respuesta Esperada__:  

Utilizando AND:  
_SELECT * FROM ARTICULOS_   
_WHERE PRECIO >= 60 AND PRECIO <=120_  

Utilizando BETWEEN:  
_SELECT * FROM ARTICULOS_  
_WHERE PRECIO BETWEEN 60 AND 120_

### **5) Obtener el NOMBRE y el PRECIO convertido a ARS (Pesos argentinos) con una relación 1 USD = 300 ARS. Para esta última, cree una columna con el nombre PrecioARS**

__Respuesta Esperada__:  
 
_SELECT NOMBRE, PRECIO * 300 AS PrecioARS FROM ARTICULOS_   

