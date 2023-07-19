<h1>TIPS: Technical Interview Preparation</h1>
<h2>Grupo A --&gt; Primer Set de Tips con Respuestas</h2>
<h2>NO MOSTRAR A SUS PAREJAS DE TIPS!</h2>
<h3>1)  Respuesta:</h3>
<p>Un JOIN interno en SQL devuelve solo los registros que tienen coincidencias en ambas tablas, mientras que un JOIN externo devuelve todos los registros de una tabla y los registros coincidentes de otra tabla. </p>
<h3>2)  Respuesta:</h3>
<p>Hay dos tipos de alcances que tienen las variables en Python. Las variables locales están declaradas dentro de una función, no puede ser llamada desde el espacio global (fuera de la función). Las variables globales, están declaradas en el espacio global (entorno) y pueden ser llamadas dentro de distintas funciones dentro del mismo entorno. </p>
<h3>3)  Respuesta:</h3>
<p>```def obtener_impares_cubicos_divididos(numeros):</p>
<pre><code>impares_cubicos_divididos = [(num ** 3) / 5 for num in numeros if num % 2 != 0]
return impares_cubicos_divididos
</code></pre>
<p>numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
impares_cubicos_divididos = obtener_impares_cubicos_divididos(numeros)
print(impares_cubicos_divididos)``` </p>
<h3>4)  Respuesta:</h3>
<p>Pueden implementarse 3 tipos de filtros:</p>
<p>Filtros a nivel visualización: Filtra tanto datos como medidas calculadas, limitando la cantidad de información que puede verse en una visualización determinada.</p>
<p>Filtros a nivel página: Filtra la info en todas las visualizaciones de una página específica del reporte.</p>
<p>Filtros a nivel reporte: se aplican a todas las páginas y visualizaciones en simultáneo.</p>
<h3>5)  Respuesta:</h3>
<p>i. Casos Favorables: 6 = (1+6),(2+5),(3+4)... 
Casos Posibles: 6*6 = 36
Probabilidad = Casos Favorables/Casos Posibles = 6/36 = 0.1667</p>
<p>ii. Casos posibles = 36
Casos Favorables = 18
Probabilidad = Casos FavorablesCasos Posibles= 18/36 = 0.5</p>
<h3>6)  Respuesta:</h3>
<p>a) 8 casos favorables de 20 posibles = 8/20 =  0.4</p>
<p>b)La probabilidad de que al sacar 2 papeles al menos tenga un coche menos la probabilidad de que al sacar 2 papeles las dos sean blancas. Por lo tanto:
= 1 - P(2 Blancas)
= 1 - (12/20)*(12/20)
= 1 - 0.36
= 0.64</p>
<p>c) Tenemos la probabilidad de que al sacar 3 papeles al menos una tenga un coche menos la probabilidad de que al sacar 3 todas sean blancas. Por lo tanto:
= 1 - P(3 Blancas)
= 1 - (12/20)<em>(12/20)</em>(12/20)
= 1 - 0.216
= 0.784</p>