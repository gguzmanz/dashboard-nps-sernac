# Dashboard de Satisfacción de Usuarios (SERNAC)

## Descripción
Análisis exploratorio y visualización de datos públicos de reclamos del SERNAC para evaluar la efectividad del SERNAC a traves del NPS durante el primer semestre del 2023

## Herramientas Utilizadas
- SQL (BigQuery): Limpieza de datos, categorización de NPS y normalización de tramos de ingreso. Al ser una base pequeña y generada de una encuestas con respuestas determinadas se realizo un AED sencillo corroborando la integridad de la data sin la necesidad de requerir de PANDAS.
- Looker Studio: Visualización interactiva y reporting.

## Metodología basada en Desing Thinking
Durante mi experiencia en el analisis de datos, defini una metodologia de trabajo basada en las 5 etapas del desing thinking pero adaptadas al proceso de analisis de datos, el cual intentare trasmitir en los siguientes pasos abordados en el trabajo presentado.

1. Se busca entender el problema y empatizar con el cliente.
2. Se define claramente el objetivo del análisis, en este caso fue definir la evaluación del SERNAC a traves de sus resultados del NPS.
3. Se bocetea el dashboard a construir, con las posibles vistas de interes.
4. Se define la estructura necesaria de la base de datos para la construcción del panel.
5. Se formatea la base de datos descargadas a CSV, se cargan a BigQuery. A traves de el proceso ETL se realiza un analisis exploratorio inicial, pasando a la construcción de la base que se utilizara para el dashboard, lo que considera calculo de metricas, formateo de columnas, condicionales, etc. Una vez realizado se carga a la herramienta de visualización en este caso Looker Studio.
6. Se procede a construir el grafico definido previamente en la etapa de boceto y en el caso de requerir se calculan metricas necesarias.
7. Se evalua si el dashboard responde y resuelve la problematica inicialmente definida, en el caso que no, se recoje el feedback y se integra en la solución.

## Decisión Panel Construido
El panel principalmente muestra vista que permiten analizar los resultados del NPS de la encuesta realizada, mostrando el promedio del NPS, la cantidad de encuestados para tener clara la dimensión de esta encuesta y el porcentaje de "Promotores". Se proponen graficos para entender la dispersión del NPS, un grafico de torta para determinar el porcentaje de promotores y desertores del total (Promotor NPS >= 9, Desertor NPS <= 6, Indiferente 7-8), y a continuación se proponen graficos para ver la evolución del resultado del NPS a lo largo del primer semestre 2023 y una tabla dinamica para ver los resultados por región.

## Conclusiones
1. A lo largo del primer semestre del 2023 ha habido una mejora continua en los resultados del NPS.
2. Los encuestados tienden a votar por extremos (1 o 10) en su mayoria.
3. La población de encuestados se centra en la RM principalmente.
4. En Marzo es probable que haya una perdida de datos.
5. Bajo la hipotesis de que estadisticamente hay mas probabilidades de que una persona califique como "Detractor" el hecho de tener sobre un 50% de "Promotores" y sobre 6 (Limite superior detractor) en promedio de NPS lo consideramos buenos resultados.

## Link al Dashboard
https://lookerstudio.google.com/reporting/cc85dbca-949a-4777-9fee-8d10a1d36256

## Base de datos SERNAC
https://datos.gob.cl/dataset/encuesta-de-satisfaccion-reclamo
