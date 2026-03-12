# VH Assistance Analytics

Proyecto de analitica para casos recoordinados, enfocado en limpiar datos operativos, transformarlos y generar visualizaciones para identificar volumen, distribucion y costo.

_**Disclamer: Los datos se generaron de forma artificial usando Grok en modo experto. No tienen ninguna relación con la realidad.**_


## Grafico interactivo
[Ver gráfico interactivo](https://juanesc396.github.io/recoordination-analytics-plot.github.io/recoordination-analytics-graph.html)


## Objetivo

Construir un flujo de analisis reproducible que permita:
- Simular base de datos extraida de _Relatorios_ que indiquen recoordinacion y motivos
- Extraer casos objetivo.
- Transformacion de datos con LLMs: Gemini: Modelo: **gemini-2.5-flash**
- Visualizar indicadores de costo por tipo de caso y por franja horaria.
- Facilitar la toma de decisiones con una salida grafica clara.

## Flujo de trabajo

1. 01_clean_data.ipynb
   - Carga de datos crudos.
   - Limpieza y estandarizacion inicial.
2. 02_transform_data.ipynb
   - Transformaciones para analitica.
   - Construccion de dataset procesado.
3. 03_analytics.ipynb
   - Analisis visual integrado.
   - Generacion de grafico principal y exportacion HTML.

## Tecnologias utilizadas

- Python 3.12
- Jupyter Notebook
- pandas
- plotly


  

