<h1>TIPS: Technical Interview Preparation</h1>
<h2>Grupo A --&gt; Segundo Set de Tips con Respuestas</h2>
<h2>NO MOSTRAR A SUS PAREJAS DE TIPS!</h2>
<h3>1)  Respuesta:</h3>
<p>SELECT C.Nombre, P.Fecha
FROM Clientes C
JOIN Pedidos P ON C.ID = P.ClienteID;</p>
<h3>2)  Respuesta:</h3>
<p>Hay muchas. Entre las más utilizadas para realizar visualizaciones varias está matplotlib (de muy bajo nivel), seaborn (construida sobre matplotlib), plotly (muy completa y de alto nivel, permite simplificar mucho la sintaxis para realizar gráficos interactivos pero es computacionalmente más costosa), plotnine (muy similar a ggplot2 muy usado en el lenguaje R), Gleam (muy similar a Shiny en el lenguaje R), missingno (muy útil para lidiar con datos faltantes), leather (permite generar gráficos simples pero en formato SVG muy escalables a cualquier resolución), Bokeh (permite gráficos interactivos) y Altair (permite gráficos interactivos muy llamativos). Para mapas, pueden utilizar Plotly, Bokeh, Altair, la librería Folium permite crear mapas interactivos muy personalizables y computacionalmente más baratos que plotly, también está la librería Geoplotlib. Para los dashboards, se puede utilizar Bokeh, Dash o Streamlit. </p>
<h3>3)  Respuesta:</h3>
<p>```def es_bisiesto(anio):
    if anio % 4 == 0:
        if anio % 100 == 0:
            if anio % 400 == 0:
                return True
            else:
                return False
        else:
            return True
    else:
        return False</p>
<p>anio = 2024
if es_bisiesto(anio):
    print(anio, "es un año bisiesto")
else:
    print(anio, "no es un año bisiesto")``` </p>
<h3>4)  Respuesta:</h3>
<p>Columna Calculada:</p>
<p>Se agregan a tablas existentes mediante fórmulas DAX sobre columnas existentes
Define y almacena valores en una columna nueva sin hacer query a la fuente de datos</p>
<p>Tabla calculada:</p>
<p>Creada mediante fórmula DAX para definir todos sus valores
Puede crearse tanto en Vista Reporte como en Vista Data</p>
<p>Medidas:</p>
<p>Se realiza a través de la query.</p>
<h3>5)  Respuesta:</h3>
<p>La probabilidad de que la persona seleccionada sea del grupo A es simplemente el porcentaje de personas del grupo A en la muestra, que es del 60%. Por lo tanto, la probabilidad de que la persona seleccionada sea A es del 60%. </p>
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