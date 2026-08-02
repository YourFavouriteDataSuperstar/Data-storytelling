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
| `Mapa_de_Visualizaciones_Matplotlib.ipynb` | El notebook. Es lo único que necesitas. |
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
