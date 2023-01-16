


# Bienvenidos a las TIP's. 
Recuerda que esto es una herramienta para practicar como seria una entrevista real! Pero en un ambiente seguro :blush:<br>
Bajo ningun punto de vista queremos su compañer@ pase un mal momento! Simplemente guialo a traves de las preguntas<br>
<sub>No le des las respuestas facilmente, pero sueltale pistas si l@ ves un poco perdido@ :wink:

<br>
  
### **1) Explique brevemente qué es y para qué sirve el indexado en una BD**

__Respuesta Esperada__:   
_El indexado es una técnica que mejora la performance de una base de datos al reducir el número necesario de lecturas de datos cuando se ejecuta una query. Mediante esta estrategia de estructura se logra encontrar y acceder a datos en una BD rápidamente._

### **2) Explique que es una función de agregación y mencione al menos 5 de las más comunes**

__Respuesta Esperada__:   
_Las funciones de agregación realizan análisis estadísticos sobre número (o fechas en algunos casos). Algunas de las funciones de agregación más comunes son: Count, AVG, Max, Min, STDDEV, Varianc_

### **3) ¿Cuál es la diferencia entre los conceptos de Data Lake y Data Warehouse?**

__Respuesta Esperada__:   
_Un data lake es un repositorio centralizado que permite almacenar datos tanto estructurado como no estructurados en cualquier escala.  
Un data warehouse es una base de datos o sistema de almacenamiento especializada, diseñada para consultas rápidas de datos estructurados de manera eficiente y escalable, típicamente usado para aplicaciones de BI y analytics._


### **4)En un sobre hay 20 papeles, 8 poseen un dibujo de un coche, las restantes son blancas. Hallar la probabilidad de extraer al menos un papel con el dibujo de un coche:**

**a) Si se saca solo un papel.**  

**b) si se sacan 2 papeles.**  


__Respuesta Esperada__:   
_a)_   
  _Casos favorables: $8$&nbsp;_  
  
  _Casos posibles: $20$&nbsp;_  

  _Respuesta: $25$&nbsp;_  

_b) La probabilidad de que al sacar 2 papeles al menos tenga un coche menos la probabilidad de que al sacar 2 papeles las dos sean blancas. Por lo tanto:_  
_ $$Probabilidad = 1 - P(2 Blancas) = 1 - 12201119 = 6295$$._  

### **5) Ejercicio practico python: Comprensión de listas**

Cree un programa que imprima una lista de todas las coordenadas 3D posibles, dadas por (i,j,k), donde:  
- la suma de i+j+k no sea igual a un valor arbitrario **_n_**.
- 0 < i <= **X**;  
- 0 < j <= **Y**;  
- 0 < k <= **Z**;  

Por favor, resolver usando **únicamente** _list comprehensions_

   
`Input`: X=1; Y=1; Z=2; n=3  

`Output`: [[0, 0, 0], [0, 0, 1], [0, 0, 2], [0, 1, 0], [0, 1, 1], [1, 0, 0], [1, 0, 1],  [1, 1, 0],  [1, 1, 2]]  
<sub>Son todas las permutaciones de (X,Y,Z) cuya suma NO da _n_</sub>

__Respuesta Esperada__: 
  
```python
x = int(input())
y = int(input())
z = int(input())
n = int(input())
output = [];
abc = [];
for X in range(x+1):
    for Y in range(y+1):
        for Z in range(z+1):
            if X+Y+Z != n:
                abc = [X,Y,Z];
                output.append(abc);
print(output);
``` 

