# Cuadernos del curso

**Universidad Ean · AFPN0098 · Data Storytelling potenciado por el análisis de Machine Learning**

| Cuaderno | Para qué | Abrir |
|---|---|---|
| **¿Se va o se queda? Clasificar clientes y ponerle precio al error** | Caso de churn con 7.043 clientes reales de una telco (IBM, base pública): qué es un modelo supervisado y por qué se separa en entrenar y probar, la regresión logística como tarjeta de puntos, la matriz de confusión con precio en cada casilla, la trampa de la exactitud, precisión y cobertura, el umbral como decisión de presupuesto, el árbol de decisión en tres preguntas y el juego del umbral de la clase. Solo hay que ejecutar las celdas en orden. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YourFavouriteDataSuperstar/Data-storytelling/blob/main/Churn_telco_clasificacion.ipynb) |
| **Segmentar para decidir: K-means contra clustering jerárquico** | Caso de negocio con 2.212 clientes reales de un retail (Kaggle, CC0): cómo funcionan K-means y el jerárquico por dentro (con ejemplos paso a paso), un cuadro por cada métrica (inercia, silueta, Calinski-Harabasz, Davies-Bouldin, estabilidad y lift) y cómo comparar algoritmos, indicadores y personas por segmento, la economía de una campaña focalizada, la elección del modelo y KNN para asignar clientes nuevos. Solo hay que ejecutar las celdas en orden. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YourFavouriteDataSuperstar/Data-storytelling/blob/main/Segmentacion_clientes_clustering.ipynb) |
| **Python desde cero para contar historias con datos** | Taller introductorio para no programadores: qué es Python, los tipos de datos, qué es una librería y un abrebocas de NumPy, pandas, matplotlib, seaborn y scikit-learn, con prompts para practicar ML desde Colab. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YourFavouriteDataSuperstar/Data-storytelling/blob/main/Python_desde_cero.ipynb) |
| **Mapa de visualizaciones con Matplotlib** | Catálogo de 15 gráficas listas para reciclar, con exportación a SVG editable. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YourFavouriteDataSuperstar/Data-storytelling/blob/main/Mapa_de_Visualizaciones_Matplotlib.ipynb) |

> [!IMPORTANT]
> **Abre los cuadernos con el botón de Colab, no desde GitHub.** GitHub elimina los estilos de los notebooks por seguridad; en Colab se ven como están diseñados y se pueden ejecutar.

---

## ¿Se va o se queda? Clasificar clientes y ponerle precio al error

Una telco pierde uno de cada cuatro clientes y solo tiene presupuesto para llamar a algunos. El cuaderno entrena un modelo que le pone un puntaje de riesgo a cada cliente, traduce cada acierto y cada error a dólares y muestra que el umbral desde el que se llama no lo decide el modelo sino la economía de la oferta. No hay que escribir código.

| Sección | Contenido |
|---|---|
| 1–2 · El problema | La telco, la decisión, la economía (oferta de 2 meses, fuga de 12) y qué es aprender con la respuesta en la mano |
| 3–4 · Los datos | Carga, limpieza explicada, dónde está la fuga y la separación 80/20 |
| 5 · El modelo | La regresión logística como tarjeta de puntos, los pesos y la curva en S |
| 6–7 · Medir y decidir | La matriz de confusión con precio, la trampa de la exactitud, precisión y cobertura, el barrido de umbrales |
| 8 · Un segundo modelo | El árbol de decisión en tres preguntas y la comparación en plata |
| 9–10 · El juego y el plan | Las 20 tarjetas del juego del umbral de cada grupo y la guía del plan de retención |

Usa `telco_churn.csv`, copia exacta de la base de muestra [Telco Customer Churn](https://github.com/IBM/telco-customer-churn-on-icp4d) que publica IBM.

---

## Segmentar para decidir: K-means contra clustering jerárquico

Una cadena de retail le habla igual a todos sus clientes y solo uno de cada siete responde a sus campañas. El cuaderno descubre los tipos de cliente que tiene, compara dos modelos de agrupamiento y escoge uno con criterios de negocio. No hay que escribir código: se ejecuta celda por celda y cada paso viene explicado.

| Sección | Contenido |
|---|---|
| 1–2 · El problema | Contexto de negocio, la pregunta bien planteada, aprendizaje no supervisado y la diferencia entre K-means y KNN |
| 3–5 · Los datos | Carga, limpieza explicada, variables de negocio, exploración y por qué escalar |
| 6 · K-means | Codo e inercia, silueta por k y por qué elegir 4 segmentos aunque la silueta prefiera 2 |
| 7 · Jerárquico | Ward, dendrograma y dónde cortar el árbol |
| 8 · Métricas | Silueta, Calinski-Harabasz, Davies-Bouldin, estabilidad con remuestreo, acuerdo entre modelos y mapa PCA |
| 9 · Negocio | Perfil de cada segmento, concentración del gasto, respuesta a campañas (validación externa) y canales |
| 10 · Decidir y usar | Matriz de decisión, KNN para clasificar clientes nuevos y plan de acción por segmento |

Usa `clientes_marketing_campaign.csv`, copia exacta de [Customer Personality Analysis](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis) (A. Patel, Kaggle, licencia CC0).

---

## Python desde cero para contar historias con datos

Un taller de una sesión para quien nunca ha programado. No se sale programando: se sale **entendiendo** lo que una IA genera cuando se le pide un análisis o un modelo, y sabiendo qué pedirle.

| Sección | Contenido |
|---|---|
| 1–3 · Python | Qué es, `print`, variables, tipos de datos (texto, entero, decimal, lógico), listas, diccionarios, `if`, `for`, funciones y cómo leer un error |
| 4 · Librerías | Qué es una librería, `import ... as`, las cinco del curso y para qué sirve cada una |
| 5 · NumPy | Arreglos, operaciones en bloque, simulación con semilla |
| 6 · pandas | DataFrame, `read_csv` desde GitHub, `info`, `describe`, filtrar, columnas calculadas, `groupby` |
| 7 · matplotlib | Anatomía de una gráfica (figura, ejes, marcas, textos), barras con etiquetas, línea con referencia y anotación |
| 8 · seaborn | `barplot`, `boxplot`, `scatterplot` con `hue`, mapa de calor de correlaciones |
| 9 · scikit-learn | La receta elegir → entrenar → predecir; regresión lineal con train/test y R²; K-Means con escalado |
| 10 · Promptear ML | Las cinco partes de un prompt de análisis, una función que describe tus datos para pegar en el prompt y tres prompts para probar |
| 11 · Para llevar | Mapa de las cinco librerías y glosario de supervivencia |

Usa `datos_ejemplo_marketing.csv` (lo lee directo desde este repositorio).

---

# Mapa de visualizaciones con Matplotlib

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YourFavouriteDataSuperstar/Data-storytelling/blob/main/Mapa_de_Visualizaciones_Matplotlib.ipynb)

**Universidad Ean · AFPN0098 · Data Storytelling potenciado por el análisis de Machine Learning**

Un catálogo de **15 gráficas listas para reciclar**. Cambias tus datos, cambias los textos, ejecutas la celda y te descarga la gráfica en **SVG editable**, lista para Illustrator, Figma, Canva o PowerPoint.

No hace falta saber programar. Solo hace falta saber **qué historia quieres contar**.

> [!IMPORTANT]
> **Ábrelo con el botón de arriba, no desde GitHub.**
> GitHub elimina los estilos de los notebooks por seguridad, así que aquí se ve plano y desordenado. En Colab se ve como está diseñado, y además se puede ejecutar.

---

## Empezar en tres pasos

1. Pulsa **Open in Colab**.
2. Ejecuta la primera celda de código (**Panel de control**) con `Ctrl+Enter` — o `Cmd+Enter` en Mac.
3. Busca tu gráfica en el catálogo, cambia los datos y los textos, y ejecútala. El `.svg` se descarga solo.

Para conservar tus cambios: **Archivo › Guardar una copia en Drive**.

---

## Qué trae

| Sección | Contenido |
|---|---|
| **¿Qué gráfica uso?** | Árbol de decisión por *lo que tiene que hacer el lector*, no por tipo de gráfica |
| **Los 6 errores que restan puntos** | Escalas truncadas, pasteles mal usados, doble eje, exceso de color, sobre-etiquetar, título descriptivo |
| **Catálogo · 15 gráficas** | Cada una con ficha de *úsala cuando / no la uses si / error típico / mensaje que comunica* |
| **Recetario de anotaciones** | 5 recetas copia-y-pega: línea de meta, sombrear periodo, flecha, resaltar punto, caja explicativa |
| **Personalizar y resolver problemas** | Tabla «quiero cambiar X → dónde → cómo» y 10 problemas frecuentes |

### El catálogo

| Familia | Gráficas |
|---|---|
| **A · Comparar magnitudes** | 01 Barras verticales · 02 Barras horizontales · 03 Barras agrupadas · 04 Barras apiladas · 05 Lollipop |
| **B · Evolución en el tiempo** | 06 Línea simple · 07 Multi-línea · 08 Área |
| **C · Distribución** | 09 Histograma · 10 Boxplot · 11 Densidad |
| **D · Relación entre variables** | 12 Dispersión · 13 Burbujas |
| **E · Composición** | 14 Dona |
| **F · Ranking con énfasis** | 15 Ranking con anotación |

---

## Archivos del repositorio

| Archivo | Para qué sirve |
|---|---|
| `Python_desde_cero.ipynb` | El taller introductorio de Python y las cinco librerías. |
| `Mapa_de_Visualizaciones_Matplotlib.ipynb` | El catálogo de 15 gráficas. |
| `datos_ejemplo_marketing.csv` | 240 filas de datos de marketing ficticios, para practicar la carga de archivos. |

---

## Cómo está construido

- **Paleta accesible** probada para daltonismo, con topes de series por tipo de gráfica (máx. 3 en dispersión y burbujas, máx. 4 en barras y líneas).
- **Modo híbrido de datos**: cada celda trae datos de ejemplo escritos a mano —así funciona siempre— y debajo, comentado, el bloque para conectar tu propio CSV cambiando solo los nombres de columna.
- **Exporta en SVG** con el texto editable, para que un diseñador pueda retocar la gráfica sin volver a Colab.
- **Funciona también fuera de Colab**: detecta el entorno y desactiva subida, descarga y Drive en un Jupyter local. Requiere `matplotlib`, `pandas`, `numpy` y `scipy`.

## Referencias

Knaflic, C. N. (2015). *Storytelling with Data*. Wiley.
Cairo, A. (2019). *How Charts Lie*. W. W. Norton.
Dykes, B. (2020). *Effective Data Storytelling*. Wiley.
