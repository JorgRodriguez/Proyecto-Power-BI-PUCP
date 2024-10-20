![Image](Imagenes/1 Inicio.png)

Link hacia el archivo Power BI:

# **CASO DE NEGOCIO**

## **OBJETIVO:** 
Desde la Temporada 1 del 2023 (1 de Abril al 30 de Junio), la empresa 123 cuenta con INDICADOR DIARIO PROMEDIO DE RENDIMIENTO DE HARINA DE PESCADO del 23% (semáforo rojo), la nueva gerencia se ha propuesta incrementar dicho indicador a 24% (semáforo verde) para el 1 de octubre de 2024

## **ESTRATEGIA:** 
Para lograr este objetivo se plantea implementar una estrategia de mejora tecnológica en el área de "ENFRIAMIENTO" logrando incrementar en promedio 15 TON de producción de Harina de pescado diaria, de una producción promedio de harina 345 TON que corresponde a una cantidad promedio de 1500 TON de materia prima diaria, sin incrementar el requerimiento de materia prima. Se realizará un product update

## **COSTO BENEFICIO:** 
El costo total de implementación de esta estrategia es de 400 KUSD. Se estima que al cumplir este objetivo en la fecha propuesta, la facturación adicional diaria será de USD 16 500, lo cual sumaria 1.485 Millones de dólares de facturación adicional solamente durante la próxima temporada (del 1 de octubre al 31 de diciembre del 2024- aproximadamente 90 días), posterior a la fecha de cumplimiento del objetivo.

# **INDICADOR**
![image]()

# **DASHBOARD**
![image]()

# **REPORTE**
![image]()

# **CREACIÓN DE TABLAS**

Para la creación de tablas y datos que alimentan el dashboard en POWER BI, se usó la aplicación de SQL Server Management (Ver archivo "SQL_Script.sql").
Para ello se usaron los datos ubicados en los archivos "datos_2023.xlsx" y "datos_2024.xlsx".

![image]()

# **CONCIDERACIONES POWER BI**

## **MANEJO DE DATOS DATE** 
Para gestionar los datos de tipo Fecha, se creó una Tabla Tiempo que permitió ajustar los períodos de análisis al construir las visualizaciones. Dado que el negocio se mide por temporadas, se incluyó una columna para clasificar las temporadas dentro de un año, lo cual fue un aspecto clave para utilizar selectores y responder las diferentes preguntas. Se adjunta el codigo en el archivo TablaTiempo.txt

![image]()

# **PANTALLAS DE APLICACIÓN**

## **PREGUNTA 1** 
![image]()

La pregunta número 1 tiene como objetivo definir si es que existe alguna estacionalidad respecto al día de la semana con mejores rendimientos para que sea un punto de partida y así analizar otras variables que puedan estar influyendo al indicador.
Utilizamos una tabla que ordenamos de manera decreciente porque las diferencias entre los valores no eran tan notorias, así como colores de diversa intensidad.

## **PREGUNTA 2** 
![image]()

La pregunta número 2 tiene como objetivo obtener una lista de los diez mejores días de producción para identificar y clasificar los días más destacados.
Utilizamos una tabla que lo ordenamos de manera decreciente porque las diferencias entre los valores no eran tan notoria, así como colores de diversa intensidad.

## **PREGUNTA 3** 
![image]()

La pregunta número 3 tiene como objetivo determinar el promedio del índice diario de producción de harina de pescado obtenido durante las temporadas **2023-T1**, **2023-T2** y **2024-T1**. Este análisis es crucial para evaluar si el rendimiento de la producción se encuentra dentro de los niveles esperados o si hay una disminución significativa que pueda requerir acciones correctivas. Utilizamos una tabla que presenta los rendimientos de cada una de las temporadas seleccionadas, junto con una tarjeta que muestra el promedio general de las mismas.
 
## **PREGUNTA 4** 
![image]()

La pregunta número 4 busca identificar cuál fue el mes del año 2023 con el mayor índice diario de rendimiento de producción de harina de pescado. Este tipo de análisis es importante para entender en qué momento del año se alcanzan los mejores niveles de eficiencia en la producción. Para responder a la pregunta, se utilizó una visualización que incluye una tabla de meses y porcentaje de rendimiento para cada mes, destacando que el rendimiento más alto se registró en octubre con un 23.004%

## **PREGUNTA 5** 
![image]()

la pregunta número 5 tiene como objetivo analizar el comportamiento entre temporadas del indicador
de rendimiento de harina de pescado para la temporada **2023-1** y **2024 -1**.
Para responder a esta pregunta optamos por un grafico de tabla ordenado de manera decreciente para facilitar el
análisis de los datos, además de una tarjeta para facilitar la visibilidad de la diferencia entre ambas
temporadas.

## **PREGUNTA 6** 
![image]()

La pregunta número 6 tiene como objetivo identificar cual de las plantas de la empresa ABC (Oeste o Norte)
cuenta con un mayor rendimiento de harina de pescado para las temporadas 2023-1 y 2023-2.
Para responder esta pregunta elegimos un grafico de tabla ordenada de manera decreciente que nos
facilita determinar cual de las plantas mencionadas cuenta con un mayor indicador para el 2023.

## **PREGUNTA 7** 
![image]()


La pregunta 7 tiene como finalidad mostrar los clientes a los que más toneladas de harina de pescado se vende, esto don el objetivo de identificar a los clientes más valiosos o rentables, permitiendo enfocar estrategias comerciales y de fidelización en estos.
Para ello se usó el gráfico de barras, el cual permite una comparación visual rápida de las ventas realizadas al TOP 5 de clientes a partir de la longitud de las barras.

## **PREGUNTA 8** 
![image]()

La pregunta número 8 busca determinar el porcentaje del total de días de producción en 2023 en los que no se alcanzó el rendimiento mínimo esperado del **23.5%**. Además, se elaboraron dos gráficos de barras independientes y similares para cada una de las dos plantas, lo que permite visualizar las diferencias de rendimiento entre ellas. Los gráficos de columnas se colorearon en rojo, amarillo y verde, representando los días en los que el indicador estuvo por debajo del **23.5%**, los días en los que se situó entre el **23.5%** y el **24%**, y los días en los que se alcanzó el **24%**, respectivamente.

## **PREGUNTA 9** 
![image]()

La pregunta número 9 tiene como objetivo identificar el impacto que tuvo el modificar el proceso de "ENFRIAMIENTO", al comparar el producto del proceso antiguo (Harina de pescado), con el generado a partir del nuevo (Harina de Pescado P2), y evaluar la diferencia en porcentaje del rendimiento obtenido en cada uno de estos.


Se usaron 2 tipos de gráficos:  
**Tabla**: Permite visualizar el detalle por mes, así como también diferenciar los productos a partir de un formato condicional  
**Tarjeta**: Hace "highlight" de los indicadores, permitiendo realizar una comparación visual rápida entre estos.

## **PREGUNTA 10** 
![image]()

El objetivo de la pregunta 10 es identificar si existe una tendencia en la producción lo largo de la semana, esto con la finalidad de evaluar día por día las razones del alto/bajo rendimiento obtenido, replicar mejores prácticas y realizar ajustes en caso aplique.


Se usaron 2 tipos de gráficos:  
**Lineal**: Muestra perfectamente la tendencia al conectar puntos de datos de manera continua, facilitando la visualización de cambios y patrones a lo largo del tiempo  
**Tabla**: Haciendo uso del formato condicional, permite comparar fácilmente los días de mayor producción de cada producto, evaluando si hay días TOP de producción en común.
