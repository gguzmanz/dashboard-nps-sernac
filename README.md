# Dashboard de Satisfacción de Usuarios (SERNAC)

## Descripción
Análisis exploratorio y visualización de datos públicos de reclamos del SERNAC para evaluar la efectividad del SERNAC a traves del NPS y buscar relaciones en la satisfacción de usuarios según tramo de ingreso y la edad de los encuestados.

## Herramientas Utilizadas
- SQL (BigQuery): Limpieza de datos, categorización de NPS y normalización de tramos de ingreso. Al ser una base pequeña y generada de una encuestas con respuestas determinadas se realizo un AED sencillo corroborando la integridad de la data sin la necesidad de requerir de PANDAS.
- Looker Studio: Visualización interactiva y reporting.

## Metodología basada en Desing Thinking
Durante mi experiencia en el analisis de datos, defini una metodologia de trabajo basada en las 5 etapas del desing thinking pero adaptadas al proceso de analisis de datos, el cual intentare trasmitir en los siguientes pasos abordados en el trabajo presentado.

1. Se busca entender el problema y empatizar con el cliente.
2. Se define claramente el objetivo del análisis, en este caso fue definir la evaluación del SERNAC a traves de sus resultados del NPS.
3. Se bocetea el dashboard a construir, con las posibles vistas de interes.
4. Se define la estructura necesaria de la base de datos para la construcción del panel.
5. Se formatea la base de datos a traves de el proceso ETL, realizando un analisis exploratorio inicial, pasando a la construcción de la base que se utilizara para el dashboard, lo que considera calculo de metricas, formateo de columnas, condicionales, etc. Una vez realizado se carga a la herramienta de visualización en este caso Looker Studio
6. Se procede a construir el grafico definido previamente en la etapa de boceto y en el caso de requerir se calculan metricas necesarias.
7. Se evalua si el dashboard responde y resuelve la problematica inicialmente definida, en el caso que no, se recoje el feedback y se integra en la solución.

## Link al Dashboard
https://lookerstudio.google.com/reporting/cc85dbca-949a-4777-9fee-8d10a1d36256

## Base de datos SERNAC
https://datos.gob.cl/dataset/encuesta-de-satisfaccion-reclamo
