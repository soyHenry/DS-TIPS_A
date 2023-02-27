<h1>TIPS: Technical Interview Preparation</h1>
<h2>Grupo A --&gt; Segundo Set de Tips con Respuestas</h2>
<h2>NO MOSTRAR A SUS PAREJAS DE TIPS!</h2>
<p><img alt="henry" src="https://blog.soyhenry.com/content/images/2021/02/HEADER-BLOG-NEGRO-01.jpg" /> </p>
<p>Esto servirá para tus entrevistas laborales asi que ¡actúa como que estuvieras en una! :bowtie: </p>
<h2>Elegir la opción correspondiente</h2>
<h3>1)  Explique que es una función de agregación y mencione al menos 5 de las más comunes.</h3>
<p>Las funciones de agregación realizan análisis estadísticos sobre número (o fechas en algunos casos. Count, AVG, Max, Min, STDDEV, Variance. </p>
<h3>2)  ¿Qué librerías de visualización para Python conoce? ¿Y para graficar mapas geográficos? ¿Y para realizar Dashboards?</h3>
<p>Hay muchas. Entre las más utilizadas para realizar visualizaciones varias está matplotlib (de muy bajo nivel), seaborn (construida sobre matplotlib), plotly (muy completa y de alto nivel, permite simplificar mucho la sintaxis para realizar gráficos interactivos pero es computacionalmente más costosa), plotnine (muy similar a ggplot2 muy usado en el lenguaje R), Gleam (muy similar a Shiny en el lenguaje R), missingno (muy útil para lidiar con datos faltantes), leather (permite generar gráficos simples pero en formato SVG muy escalables a cualquier resolución), Bokeh (permite gráficos interactivos) y Altair (permite gráficos interactivos muy llamativos). Para mapas, pueden utilizar Plotly, Bokeh, Altair, la librería Folium permite crear mapas interactivos muy personalizables y computacionalmente más baratos que plotly, también está la librería Geoplotlib. Para los dashboards, se puede utilizar Bokeh, Dash o Streamlit. </p>
<h3>3)  ¿Qué es NumPy? ¿Cuál es la estructura de datos que utiliza y en qué se diferencia de una lista?</h3>
<p>NumPy es un paquete de módulos muy popular en Python, que permite realizar operaciones matemáticas y algebraicas muy fácil y eficientemente, gracias a su estructura de datos, llamada Array (o arreglo) que, al tener sólo un tipo de dato (a diferencia de las listas que pueden tener al mismo tiempo strings, floats, e incluso diccionarios o listas) permite trabajar mucho más eficientemente y aparte permite almacenar datos en varias dimensiones </p>
<h3>4)  ¿Cuál es la diferencia entre medida calculada, columna calculada y tabla calculada?</h3>
<p>Columna Calculada:
Se agregan a tablas existentes mediante fórmulas DAX sobre columnas existentes
Define y almacena valores en una columna nueva sin hacer query a la fuente de datos
Tabla calculada:
Creada mediante fórmula DAX para definir todos sus valores
Puede crearse tanto en Vista Reporte como en Vista Data
Medidas:
Se realiza a través de la query</p>
<h3>5)  En un sobre hay 20 papeles, 8 poseen un dibujo de un coche, las restantes son blancas. Hallar la probabilidad de extraer al menos un papel con el dibujo de un coche:</h3>
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
<h3>6)  Se sacan dos bolas de una urna que se compone de una bola blanca, otra roja, otra verde y otra negra. Describa el espacio muestral cuando:</h3>
<p>a) La primera bola se devuelve a la urna antes de sacar la segunda.
b) La primera bola no se devuelve.</p>
<p>a) E = {BB,BR,BV,BN,RB,RR,RV,RN,VB,VR,VV,VN,NB,NR,NV,NN}
b) E={BR,BV,BN,RB,RV,RN,VB,VR,VN,NB,NR,NV} </p>
