<h1>TIPS: Technical Interview Preparation</h1>
<h2>Grupo A --&gt; Primer Set de Tips con Respuestas</h2>
<h2>NO MOSTRAR A SUS PAREJAS DE TIPS!</h2>
<h3>1)  Respuesta:</h3>
<p>INNER JOIN: Devuelve todas las filas cuando hay al menos una coincidencia en ambas tablas.</p>
<p>LEFT JOIN: Devuelve todas las filas de la tabla IZQUIERDA y las filas coincidentes de la tabla de la derecha.</p>
<p>RIGHT JOIN: Devuelve todas las filas de la tabla DERECHA y las filas coincidentes de la tabla de la izquierda.</p>
<p>OUTER JOIN: Devuelve todas las filas de las dos tablas. También conocida como FULL OUTER JOIN.</p>
<h3>2)  Respuesta:</h3>
<p>Las VARIABLES CATEGÓRICAS son un tipo de dato que maneja nativamente pandas (type=category). Una variable categórica toma solo una categoría fija(generalmente un número fijo) de valores. Algunos ejemplos de variables categóricas son género, grupo sanguíneo, idioma, etc. Un contraste principal con estas variables es que no se pueden realizar operaciones matemáticas con estas variables. </p>
<h3>3)  Respuesta:</h3>
<p>```import random</p>
<p>def dados():
    dado1 = random.randint(1, 7)
    dado2 = random.randint(1, 7)</p>
<pre><code>if dado1 &gt; dado2:
    print(dado1, dado2)
    return "Jugador con dado 1 gana"

elif dado1 &lt; dado2:
    print(dado1, dado2)
    return "Jugador con dado 2 gana"
else:
    print(dado1, dado2)
    return "Empate"
</code></pre>
<p>dados()``` </p>
<h3>4)  Respuesta:</h3>
<p>Hay 3 tipos de vistas disponibles, cada una con un propósito diferente:</p>
<p>Vista Reporte: permite añadir páginas, visualizaciones y publicar</p>
<p>Vista de Data: permite realizar manejo de datos usando herramientas de Query Editor</p>
<p>Vista de Modelo: permite manejar las relaciones entre las tablas de datos</p>
<h3>5)  Respuesta:</h3>
<p>La probabilidad de que la persona seleccionada sea del grupo A es simplemente el porcentaje de personas del grupo A en la muestra, que es del 60%. Por lo tanto, la probabilidad de que la persona seleccionada sea A es del 60%. </p>
<h3>6)  Respuesta:</h3>
<p>La probabilidad condicional es la probabilidad de que un evento ocurra dado que otro evento ya ha ocurrido. La probabilidad condicional se calcula dividiendo la probabilidad del evento conjunto por la probabilidad del evento condicionante. </p>