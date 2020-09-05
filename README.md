# TFM-Javier_Casado : Audience Forecasting


## Introducción

El presente proyecto busca desarrollar una herramienta que permita realizar predicciones certeras sobre la audiencia futura en una cadena de televisión determinada. La idea para este proyecto surge a raiz de la problemática que encuentran los planificadores de medios cuando gestionan campañas publicitarias de los clientes. Estas campañas se pagan en función de la gente que vea el spot publicitario. Es por eso que necesitan una estimación lo más aporximada posible a la audiencia real, para getionar la campaña sin salirse de los costes estipulados y cumpliendo requerimientos de los clientes.
Este proyecto busca abordar de una manera simple y clara los problemas mencionados. En todo momento se ha buscado optimizar tanto código como archivos necesarios para la ejecución del proyecto.


## Contenido del repositorio

Este apartado explica que contiene el repositorio y lo que se ha ido haciendo en cada uno de los notebooks. Se ha procurado simplificar al máximo la organización del mismo, aunando el código y las visualizaciones finales en cada uno de los cinco archivos presentes:

1. Data_processing.ipynb: este notebook contiene el procesado y limpieza de datos inicial. Tras ejecutar el presente notebook, se obtiene como resultado un dataset con todas las variables necesarias para realizar el apartado de visualización y para entrenar el algoritmo. Es en este punto donde se crean columnas complementarias a las contenidas en los datos originales. Algunas de estas columnas se crean para la visualización exclusivamente, y carecen de sentido en la fase de modelización.

2. Model.ipynb: en este caso, el notebook contiene la fase de busqueda y entrenamiento del modelo. Para este apartado es necesario tener el dataset resultante del notebook anterior. Aquí se valoran varios modelos a través del error medio absoluto y el error cuadrático medio. También se prueba diferentes configuraciones para el modelo seleccionado, utilizando las mismas métricas mencionadas anteriormente.

3. Visualization.pbix: este archivo busca aportar al proyecto un entorno donde visualizar las métricas y datos necesarios para la correcta planificación de una campaña, así como mostrar los datos resultantes de una predicción determinada. También sirve como herramienta para el control de datos, y para comprobar que la fase de carga y limpieza de datos se ha realizado correctamente. A través de este archivo no solo podremos visualizar datos relevantes, sino que también servirá para hacer seguimiento de los datos disponibles.

4. Project_report.pdf: el documento que recoge todos los pasos seguidos en el proyecto. En él se explica en detalle las decisiones tomadas en cada apartado, y se explican los datos disponibles. Se recomienda encarecidamente su lectura antes de proceder con el resto de archivos.

5. Visualization_manual.pdf: este archivo contiene la explicación de todo el módulo de visualización. En él se explica la importancia de los diferentes análisis realizados, así como todo el control de la carga de datos.

No ha sido posible cargar en el repositorio la totalidad de los datos utilizados (130GB aprox). Podrá disponer de los datos contactando con el propietario del proyecto.


## Tecnologías utilizadas

El proyecto se ha realizado casi en su totalidad haciendo uso de los notebooks de Jupyter, y utilizando python como lenguaje de programación. Para la parte de visualización se ha utilizado la herramienta para dashbords interactivos, Power BI.


## Workflow

Como se mencionó anteriormente, se recomienda en primer lugar la lectura de la memoria, para comprender mejor las decisiones tomadas. Para poder llegar a los resultados esperedas, se deberá ejecutar primero el notebook de procesado y limpieza de datos, para posteriormente pasar al notebook de modelado, usando el dataset resultado de la primera ejecución. Para el documento de visualización habrá que cargar el dataset resultante de la ejecución de los dos notebooks(df_ml_21.csv).
