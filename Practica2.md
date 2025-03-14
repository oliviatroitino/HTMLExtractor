#### Práctica 2: Categorizador de Documentos

#### Objetivo:

Los alumnos individualmente han de analizar la efectividad del resumen como método de explicación de los tópicos resultantes de la técnica LDA sobre páginas de Wikipedia. La técnica LDA clasifica documentos en un número de tópicos fijo que se asignan durante la ejecución del algoritmo en base a la frecuencia de términos entre diversos documentos. Los tópicos obtenidos de un algoritmo LDA son difíciles de interpretar. Para obtener una interpretación más fácil de los tópicos se propone en esta práctica emplear métodos de resúmenes de documentos. Se propone buscar y comparar diferentes métodos de resúmenes sobre documentos clasificados en tópicos para facilitar la interpretación de los tópicos.

## HTML Scraping
Al principio, los alumnos manualmente han de ==seleccionar una lista de URLs de páginas de Wikipedia== (más de 50) y almacenar la lista en un fichero de texto plano. Después, mediante un programa Python o Jupyter Notebook han de ==descargar páginas HTML de Wikipedia== a partir de la lista de URLs seleccionadas. Los ficheros HTML han de ==almacenarse en una carpeta de resultados de HTML==. Luego, han de procesarse dichos ficheros HTML para ==extraer los párrafos y títulos del cuerpo de los documentos== (no nos interesan índices, ni imágenes, ni enlaces). Los resultados del procesamiento han de almacenarse como ==ficheros de texto plano en otra carpeta de resultados distinta== a la carpeta de resultados de HTML.

## LDA
A continuación, en un nuevo Jupyter Notebook, los alumnos vuelven a preprocesar los documentos en texto plano para aplicarlos en la técnica de LDA. Luego, analizan las métricas de coherencia y perplejidad del modelo LDA. Analizados los resultados de estas dos métricas, escogen un número de tópicos. Después, escogido e número de tópicos, generan un gráfico empleando pyLDAvis para analizar la relación entre los tópicos presentes. Lo más importante de este análisis es identificar las palabras más importantes de cada tópico e identificar la superposición de los tópicos. Una vez analizado el resultado del LDA según las recomendaciones de la métrica de perplejidad y coherencia, se puede generar otro análisis empelando un número de tópicos arbitrario diferente del anterior análisis si se considera que se obtienen mejores resultados en la práctica. Como mínimo, es necesario un análisis basado en el número de tópicos deducido de las métricas de coherencia y perplejidad.

## Resúmenes por Tópico
Finamente, del mejor resultado del número de tópicos se clasifican los documentos según los tópicos obtenidos y se genera un resumen por cada tópico. Para llevar a cabo este resumen se pueden emplear diversas técnicas, tanto basadas en Deep Learning como las basadas en frecuencia de términos o TextRank. Tras obtener el resultado de los resúmenes, razonar si se pudiera empelar el resumen en cada caso como explicación del tópico y escribir al menos un párrafo de conclusiones sobre los resultados y los métodos empleados en esta práctica.

#### Instrucciones:

1. Implementar un extractor y procesador de HTML de Wikipedia a partir de una lista de URLs.
2. Implementar un Jupyter Notebook que:
3. Procesa los datos de texto plano extraídos de Wikipedia como entrada de un LDA.
4. Obtiene gráficas de coherencia y perplejidad para LDA para múltiples números de tópicos.
5. Explica la gráfica de pyLDAvis con el número de tópicos elegido.
6. Resume los documentos de los tópicos.
7. Justificar los pasos llevados a cabo en las fases anteriores y escribir las conclusiones.

#### Evaluación:

1. Extractor de HTML de Wikipedia (1 punto).
2. Procesador de HTML (1 puntos).
3. Procesador de Texto Plano para LDA (1 puntos).
4. Analizador de coherencia y perplejidad (1 puntos).
5. Análisis del resultado pyLDAvis (2 puntos).
6. Análisis de los resúmenes de los tópicos (2 puntos).
7. Conclusiones sobre el proyecto y claridad general (2 punto).

#### Entregables:

1. Extractor y procesador de HTML de Wikipedia en formato Jupyter Notebook (.ipynb).
2. Generador de análisis documentado en formato Jupyter Notebook (.ipynb)
3. Fichero con las URLs en formato de texto plano (.txt).
4. Fichero comprimido con la carpeta de resultados del extractor de HTML (.zip). El fichero contiene una carpeta con 50 o más ficheros de tipo html (.html).
5. Fichero comprimido con la carpeta de resultados del procesador de HTML (.zip). El fichero contiene una carpeta con 50 o más ficheros de texto plano (.txt).
6. (Opcional) Fichero llamado “README.md” que contendrá documentación sobre como ejecutar y preparar la ejecución de la práctica o sobre como están organizados los ficheros.

#### Notas:

- Los alumnos que entreguen una práctica que dé un error no controlado o no documentado (en un fichero llamado “README.md”), estará automáticamente suspensa con un cero. Entre estos errores se consideran los siguientes:
- Excepciones que no se atrapan ni se documentan.
- Errores de codificación.
- Errores de importación del código como librería.
- Las entregas fuera de la fecha final de la práctica se consideran suspensas y su valoración será un cero.
- Las entregas que empleen librerías no vistas en clase, han de documentar las librerías que hay que instalar y el comando con el que se instalan en un fichero aparte llamado “README.md”. Si aparecen librerías no vistas en clase sin ser documentadas en este fichero, el valor de la práctica será de cero.