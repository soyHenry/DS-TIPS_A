<h1>TIPS: Technical Interview Preparation</h1>
<h2>Grupo A --&gt; Primer Set de Tips con Respuestas</h2>
<h2>NO MOSTRAR A SUS PAREJAS DE TIPS!</h2>
<p><img alt="henry" src="https://blog.soyhenry.com/content/images/2021/02/HEADER-BLOG-NEGRO-01.jpg" /> </p>
<p>Esto servirá para tus entrevistas laborales asi que ¡actúa como que estuvieras en una! :bowtie: </p>
<h2>Elegir la opción correspondiente</h2>
<h3>1)  Explique la diferencia entre la cláusula WHERE y la cláusula HAVING</h3>
<p>La cláusula WHERE es utilizada para aplicar condiciones/filtros ANTES de aplicar cualquier agregación (o cuando no se aplique ninguna). La cláusula HAVING es usada para aplicar condiciones/filtros DESPUÉS de dar lugar a la agregación. </p>
<h3>2)  ¿Qué es un index en Pandas? ¿Cómo podría acceder a él? ¿Puede haber más de uno?</h3>
<p>El 'index' es el "índice" de DataFrame, se aplica normalmente a la referencia de un dato en una estructura según su posición, para poder referenciar cada fila. Se puede acceder a través del atributo .index de pandas, que devuelve la representación del mismo. Puede haber más de un índice en el DataFrame, estas estructuras poseen MultiIndex, que es un índice funcionando a varios niveles de jerarquía, donde múltiples columnas de índice refieren a una fila. Permiten análisis de datos multidimensionales. </p>
<h3>3)  ¿Qué librerías de visualización para Python conoce? ¿Y para graficar mapas geográficos? ¿Y para realizar Dashboards?</h3>
<p>Hay muchas. Entre las más utilizadas para realizar visualizaciones varias está matplotlib (de muy bajo nivel), seaborn (construida sobre matplotlib), plotly (muy completa y de alto nivel, permite simplificar mucho la sintaxis para realizar gráficos interactivos pero es computacionalmente más costosa), plotnine (muy similar a ggplot2 muy usado en el lenguaje R), Gleam (muy similar a Shiny en el lenguaje R), missingno (muy útil para lidiar con datos faltantes), leather (permite generar gráficos simples pero en formato SVG muy escalables a cualquier resolución), Bokeh (permite gráficos interactivos) y Altair (permite gráficos interactivos muy llamativos). Para mapas, pueden utilizar Plotly, Bokeh, Altair, la librería Folium permite crear mapas interactivos muy personalizables y computacionalmente más baratos que plotly, también está la librería Geoplotlib. Para los dashboards, se puede utilizar Bokeh, Dash o Streamlit. </p>
<h3>4)  ¿Qué tipo de filtros pueden implementarse en POWER BI?</h3>
<p>Pueden implementarse 3 tipos de filtros:
Filtros a nivel visualización: Filtra tanto datos como medidas calculadas, limitando la cantidad de información que puede verse en una visualización determinada.
Filtros a nivel página: Filtra la info en todas las visualizaciones de una página específica del reporte.
Filtros a nivel reporte: se aplican a todas las páginas y visualizaciones en simultáneo.</p>
<h3>5)  Una urna tiene ocho bolas rojas, cinco amarillas y siete verdes. Si se extrae una bola al azar calcular la probabilidad de que:</h3>
<p>i. No sea Roja
ii. No sea Verde
iii. Sea Amarilla</p>
<p>i.Casos Favorables: 12
Casos posibles: 8 + 5 + 7 = 20
Probabilidad = Casos FavorablesCasos Posibles= 1220 = 0.6
ii. Casos Favorables: 13
Casos posibles: 8 + 5 + 7 = 20
Probabilidad = Casos FavorablesCasos Posibles= 1320 = 0.65
iii. Casos Favorables: 5
Casos posibles: 8 + 5 + 7 = 20
Probabilidad = Casos FavorablesCasos Posibles= 520 = 0.25 </p>
<h3>6)  En un sobre hay 20 papeles, 8 poseen un dibujo de un coche, las restantes son blancas. Hallar la probabilidad de extraer al menos un papel con el dibujo de un coche:</h3>
<p>a) Si se saca solo un papel.
b) Si se extraen dos papeles.
c) Si se extraen 3 papeles.</p>
<p>a) 8 casos favorables de 20 posibles. RTA 25
b)La probabilidad de que al sacar 2 papeles al menos tenga un coche menos la probabilidad de que al sacar 2 papeles las dos sean blancas. Por lo tanto:
= 1 - P(2 Blancas)
= 1 - 12201119
= 6295
c) Tenemos la probabilidad de que al sacar 3 papeles al menos una tenga un coche menos la probabilidad de que al sacar 3 todas sean blancas. Por lo tanto:
= 1 - P(3 Blancas)
= 1 - 122011191018
= 4657</p>
