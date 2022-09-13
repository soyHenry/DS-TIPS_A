# Henry - TIPS Grupo A

## **Cuestionario**:
### **1) Nombre los diferentes objetos de una base de datos (pista: 6 son permanentes y 1 temporal).**  
__Respuesta Esperada__:   _Permanentes: Table, Views, Procedures, Functions, Triggers y Indexes. Temporales: Cursors_ 

### **2) ¿Qué es una subconsulta? Explique de manera breve su sintaxis.**
__Respuesta Esperada__:   _Una subconsulta es una consulta hecha sobre otra consulta. Su sintaxis es:_  
_SELECT <column_name> FROM <table_name>_   
_WHERE <column_name> IN/NOT IN_  
_(subconsulta)_
 

### **3) Se sacan dos bolas de una urna que se compone de una bola blanca, otra roja, otra verde y otra negra. Describa el espacio muestral cuando:**  
**a)** La primera bola se devuelve a la urna antes de sacar la segunda.  
__Respuesta Esperada__:   _E = {BB,BR,BV,BN,RB,RR,RV,RN,VB,VR,VV,VN,NB,NR,NV,NN}_   
**b)** La primera bola no se devuelve.    
__Respuesta Esperada__:   _E={BR,BV,BN,RB,RV,RN,VB,VR,VN,NB,NR,NV}_

### **4) A partir del punto anterior, calcule la probabilidad de que se extraiga una bola y no sea Roja.**  
__Respuesta Esperada__:  
_Casos Favorables: 12_  
_Casos Posibles: 20_  
_Probabilidad = 12/20 = 0.6_

### **5) Escriba las diferencias entre una Tupla y una Lista.**  
__Respuesta Esperada__:  
|  | Lista | Tupla |
|------|------|-------|
|Velocidad|Inferior|Mayor |
| Mutabilidad | Si | No |
|sintaxis  | cochetes  | parentesis|


### **6) Escriba una función que dada una lista de colores devuelva el nombre y la cantidad de veces que se repita.**
**lista = ['verde', 'rojo', 'azul', 'naranja', 'rojo', 'violeta', 'blanco', 'blanco', 'negro', 'rosa', 'marron']**

__Ejemplo de Respuesta Esperada__:  

import pandas as pd  
import numpy as np  

def funcion(color, lista):  
----cantidad = 0  
----n = 0  
----while n <= (len(lista) - 1):  
--------if lista[n] == color:  
------------cantidad = cantidad + 1  
--------n = n+1      
----return color, cantidad  

