# 📊 Informe de Análisis de Datos — Proyecto Final

## 1. Introducción

El objetivo de este proyecto es realizar un análisis exploratorio de datos (EDA) sobre un conjunto de datos de películas, combinando información de valoraciones de usuarios con características cinematográficas como presupuesto, ingresos, género o país de producción.

El análisis busca identificar patrones relevantes en la industria cinematográfica, especialmente en relación con la rentabilidad (ROI), la popularidad y la distribución geográfica de los ingresos.

---

## 2. Transformación y limpieza de los datos

El dataset original presenta una característica clave:
cada película aparece múltiples veces debido a la existencia de valoraciones de distintos usuarios.

Esto genera duplicidades que afectan directamente al análisis si no se tratan correctamente.

### Principales acciones realizadas:

* Eliminación de variables irrelevantes (IDs secundarios, columnas redundantes).
* Conversión de tipos de datos (fechas, variables numéricas).
* Tratamiento de valores nulos.
* Extracción de variables a partir de estructuras complejas:

  * `main_genre` (género principal)
  * `secondary_genre`
  * `main_country`
  * `num_countries`

### Tratamiento de duplicados

Dado que cada película aparece múltiples veces, se aplicaron las siguientes estrategias:

* Uso de **recuento distinto (`distinct count`)** para contar películas reales.
* Creación de métricas agregadas por identificador único de película (`id`).
* Cálculo de ingresos y presupuesto reales evitando duplicación.

Esto ha permitido obtener métricas fiables y evitar sobreestimaciones.

---

## 3. Análisis descriptivo de los datos

### Distribución por géneros

El análisis muestra que los géneros más frecuentes son:

* Drama
* Comedy
* Action

Esto indica una clara predominancia de ciertos géneros en la producción cinematográfica.

---

### Distribución temporal

El número de películas presenta una mayor concentración en los primeros años del dataset, con una disminución progresiva en años posteriores.

Esto puede deberse a:

* procesos de filtrado aplicados
* características del dataset original

---

### Distribución geográfica

Estados Unidos destaca como el principal país en generación de ingresos, seguido por:

* Reino Unido
* Alemania
* Francia

Esto refleja la concentración de la industria en determinados mercados.

---

## 4. Análisis estadístico de los datos

### Relación entre presupuesto e ingresos

El análisis mediante gráficos de dispersión muestra:

* Existe una relación positiva entre presupuesto e ingresos.
* Sin embargo, no es proporcional:

  * algunas películas con bajo presupuesto generan altos ingresos
  * otras con alto presupuesto no obtienen resultados equivalentes

---

### Popularidad vs valoración

No se observa una relación clara entre popularidad y valoración:

* películas muy populares no siempre son mejor valoradas
* existen películas con baja popularidad pero alta valoración

Esto indica que el éxito comercial no siempre está alineado con la percepción del público.

---

### Análisis de rentabilidad (ROI)

El ROI permite identificar películas altamente rentables.

Se observa que:

* algunas películas con presupuestos bajos generan altos niveles de rentabilidad
* las producciones más costosas no siempre son las más eficientes

---

### Coproducciones

El análisis muestra que:

* predominan las producciones únicas
* las coproducciones representan una proporción menor

Sin embargo, las coproducciones pueden estar asociadas a una mejor optimización de recursos en determinados casos.

---

## 5. Dashboard interactivo

Se ha desarrollado un dashboard en Power BI estructurado en tres páginas:

### 🔹 1. Resumen general

* KPIs principales (películas, ingresos, presupuesto, ROI, valoración)
* Distribución por género
* Evolución temporal
* Mapa de ingresos por país

---

### 🔹 2. Análisis por género y país

* Comparación ingresos vs presupuesto por género
* Distribución de coproducciones
* Ranking de países por ingresos

---

### 🔹 3. Rendimiento y popularidad

* Relación presupuesto vs ingresos
* Popularidad vs valoración
* Duración media por género
* Top películas por ROI

---

## 6. Conclusiones

A partir del análisis realizado se pueden extraer las siguientes conclusiones:

* Los géneros Drama y Comedy dominan en número de producciones.
* Estados Unidos concentra la mayor parte de los ingresos.
* No existe una relación directa entre popularidad y valoración.
* El presupuesto no garantiza el éxito económico.
* Algunas películas de bajo presupuesto presentan niveles de rentabilidad muy elevados.
* La estructura del dataset requiere un tratamiento cuidadoso para evitar duplicidades.

---

## 7. Limitaciones

* El dataset contiene duplicados por usuario que requieren tratamiento específico.
* La distribución temporal no es uniforme.
* Algunos campos complejos han sido simplificados (géneros, países).

---

## 8. Trabajo futuro

* Incorporar más variables (actores, director, etc.)
* Análisis predictivo de ingresos o éxito
* Mejora del dashboard con filtros avanzados

---
