# HTMLExtractor

## Dependencias
```
beautifulsoup4
gensim
```

# HTMLExtractor.ipynb
`HTMLExtractor.ipynb` lee el fichero `WikiURLs.txt` y guarda los URLs de Wikipedia en una lista. Después pasa por cada uno de esos links y usa `BeautifulSoup` para extraer el código HTML de los links y los guarda en el directorio `HTMLResults`.

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