![Python](https://img.shields.io/badge/Python-3.13-blue.svg)
![Project](https://img.shields.io/badge/Proyecto-Final-purple)
![Status](https://img.shields.io/badge/Dashboard-Pendiente-orange)
![Progress](https://img.shields.io/badge/Estado-En%20Progreso-yellow)

# 🎬 Análisis de Datos del Sector Cinematográfico

## 📖 Descripción del Proyecto
Este proyecto constituye el **Proyecto Final del módulo de Análisis de Datos en Python**.  
Su objetivo es realizar un **análisis exploratorio y estadístico** de un conjunto de datos cinematográficos,  
identificando patrones en la producción, la rentabilidad y las valoraciones del público.  

El análisis busca responder preguntas clave como:
- ¿Qué géneros y países destacan en número de producciones y valoración media?  
- ¿Cómo se relacionan el presupuesto, los ingresos y las valoraciones?  
- ¿Existen diferencias relevantes entre producciones únicas y coproducciones?  

Incluye todo el proceso analítico completo:
- Limpieza y transformación profunda de los datos.  
- Análisis descriptivo, comparativo y estadístico.  
- Visualizaciones interpretativas.  
- Conclusiones globales explicativas.  
- **Dashboard operativo (pendiente de implementación).**

---

## 🗂 Estructura del Proyecto

📁 Proyecto_Final/\
├── data/\
│   ├── dataset_final.zip   # Dataset limpio usado en el análisis\
├── notebooks/\
│ └── Proyecto_Final.ipynb # Notebook principal con el análisis completo\
├── README.md # Descripción del proyecto (este archivo)\

---

## 📂 Fuentes de Datos

Los datos originales utilizados en este proyecto provienen de **[The Movies Dataset (Kaggle)](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset)**, un conjunto de datos público con información sobre películas, géneros, países de producción, presupuestos, ingresos y valoraciones de usuarios.

De este dataset completo se han empleado específicamente los siguientes archivos para el análisis:

- `movies_metadata.csv` → Contiene información general de las películas (género, idioma, país, presupuesto, ingresos, etc.).  
- `ratings.csv` → Contiene las valoraciones de los usuarios a cada película.

El resto de archivos incluidos en el dataset original no se han utilizado en este proyecto.

Tras la limpieza y transformación de los datos, ambos archivos se integraron en un **dataset final procesado**, disponible en este repositorio bajo el nombre:  
📦 `dataset_final.zip`  

> 💡 Nota: Los datos originales no se incluyen directamente en el repositorio debido a su tamaño, pero pueden descargarse libremente desde el enlace de Kaggle indicado arriba.

---

## 🛠 Instalación y Requisitos

**Lenguaje:** Python 3.13  

**Librerías principales utilizadas:**
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scipy  
- json  

**Para ejecutar el proyecto:**
1. Clonar el repositorio o descargar los archivos.  
2. Abrir el notebook `Proyecto_Final.ipynb` en Jupyter o VS Code.  
3. Ejecutar las celdas en orden para reproducir todo el análisis.  

---

## 📊 Resultados y Conclusiones

### 🔹 Limpieza y Transformación
- Se eliminaron duplicados, nulos y valores inconsistentes.  
- Se transformaron columnas complejas (géneros, países, colecciones) en estructuras normalizadas.  
- Se crearon nuevas variables como `main_country`, `num_countries`, `main_genre`, `ROI`, etc.  
- Se integraron `movies_metadata` y `ratings` en un único dataset limpio.  

### 🔹 Análisis Descriptivo y Exploratorio
- **Ratings:** Distribución centrada en valores intermedios (3–4), lo que refleja valoraciones equilibradas.  
- **Géneros:** Drama, Comedy y Action dominan en volumen, pero **Animation y Documentary** obtienen mejores valoraciones medias.  
- **Países:** EE.UU. lidera en cantidad de producciones, mientras que **Reino Unido, Francia y Alemania** muestran resultados de calidad competitiva.  
- **Presupuesto vs Ingresos:** Existe una correlación positiva; sin embargo, el alto presupuesto no garantiza el éxito.  

### 🔹 Comparativa de Producciones
**Coproducciones vs Producciones Únicas:**
- Ingresos medios: **Producciones únicas ligeramente superiores** (+2.42M, +3.35%).  
- Mediana: **Coproducciones** con valores más altos (18.6M vs 0.17M).  
- ROI: **Producciones únicas más rentables** (3.84 vs 2.19).  
- Diferencia significativa (p < 0.001) en ingresos log-transformados → **producciones únicas superiores**.

**Conclusión global:**  
Las **producciones únicas** son más rentables pero arriesgadas;  
las **coproducciones** son más estables y tienden a asegurar ingresos intermedios.  

---

## 🔄 Próximos Pasos
- Implementar el **Dashboard operativo** para explorar resultados de forma interactiva.  
- Incluir nuevas métricas temporales (evolución por décadas, popularidad anual).  
- Ampliar el análisis con variables de audiencia o sentimiento en reseñas.  

---

## 📊 Dashboard Operativo

El proyecto se complementará con un **Dashboard interactivo**, cuyo objetivo es facilitar la interpretación visual de los resultados y permitir una exploración dinámica de las principales métricas del análisis.

Inicialmente, el dashboard se desarrollará en **Power BI**, aunque se contempla la posibilidad de implementarlo en **Google Sheets** si la herramienta resulta más adecuada para la visualización final.

El panel incluirá visualizaciones centradas en los siguientes ejes de análisis:

- Distribución de valoraciones por género y país  
- Relación entre presupuesto e ingresos  
- Rentabilidad (ROI) y su comparación entre producciones únicas y coproducciones  
- Evolución temporal de valoraciones y volumen de producciones  

📎 **Estado actual:** en desarrollo  
🔗 Una vez finalizado, el dashboard estará disponible para su consulta mediante enlace público, que se añadirá en esta sección del README.


---

## ✒ Autora
**Celia Palacios**  
💻 Proyecto Final   

---

## 🧾 Nota Final
El notebook `Proyecto_Final.ipynb` actúa como **informe explicativo completo**,  
incluyendo la limpieza, análisis, visualización y conclusiones globales.  
Solo falta la implementación del **Dashboard operativo** para completar el proyecto.
