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
├── data/ # Datos crudos y dataset limpio final\
├── notebooks/\
│ └── Proyecto_Final.ipynb # Notebook principal con el análisis completo\
├── README.md # Descripción del proyecto (este archivo)\
└── results/ # Gráficos o resultados exportados (opcional)

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

## ✒ Autora
**Celia Palacios**  
💻 Proyecto Final   

---

## 🧾 Nota Final
El notebook `Proyecto_Final.ipynb` actúa como **informe explicativo completo**,  
incluyendo la limpieza, análisis, visualización y conclusiones globales.  
Solo falta la implementación del **Dashboard operativo** para completar el proyecto.
