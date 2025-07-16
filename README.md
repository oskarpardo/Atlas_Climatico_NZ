# 📈 Atlas de Adaptación Agro-Climática de Nueva Zelanda para 2050

![Python](https://img.shields.io/badge/python-3.x-blue.svg) ![Pandas](https://img.shields.io/badge/pandas-2.x-blue.svg) ![NumPy](https://img.shields.io/badge/numpy-1.2x-blue.svg) ![Streamlit](https://img.shields.io/badge/streamlit-1.x-orange.svg) ![Plotly](https://img.shields.io/badge/plotly-5.x-orange.svg) ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

**Un proyecto de análisis de datos de ciclo completo para evaluar el riesgo climático y modelar estrategias de adaptación en las industrias primarias clave de Nueva Zelanda.**

---

### ➡️ [Ver Dashboard Interactivo en Vivo](link vacio por ahora)

*Aquí se insertará una GIF animada del dashboard final en acción para una demostración visual inmediata.*

---

## 1. Visión del Proyecto y Propuesta de Valor

Este proyecto simula un encargo de consultoría estratégica de alto nivel, diseñado para ir más allá del análisis de datos convencional. El objetivo es construir un prototipo de **Herramienta de Evaluación de Riesgo Climático**. La propuesta de valor es demostrar la capacidad de transformar datos dispares y complejos en una herramienta interactiva que facilita la toma de decisiones estratégicas a largo plazo. El resultado final no solo presenta hallazgos, sino que ofrece una solución que un stakeholder, como un viticultor o un planificador gubernamental, puede utilizar para explorar escenarios y planificar la adaptación.

## 2. El Problema de Negocio

Las industrias primarias son la columna vertebral de la economía de exportación de Nueva Zelanda, definiendo la identidad productiva del país. Sin embargo, enfrentan una amenaza tangible y creciente por el cambio climático. Este proyecto aborda los siguientes riesgos específicos y medibles:

* **Viticultura:** El calentamiento global está causando una "compresión de la cosecha", acelerando la maduración de la uva, lo que afecta su calidad y crea cuellos de botella logísticos durante la vendimia.
* **Kiwis:** El aumento de las temperaturas invernales amenaza con la "pérdida de frío invernal". Las variedades de kiwi como Hayward necesitan un número mínimo de horas a bajas temperaturas para una brotación y cosecha abundantes, poniendo en riesgo la viabilidad del cultivo en regiones clave como Bay of Plenty.
* **Lechería:** El incremento de "días de estrés por calor" (temperaturas > 25°C) puede reducir la ingesta de alimento del ganado, disminuir la producción de leche y afectar la salud general de los animales.

## 3. Hipótesis de Investigación

Para abordar este problema, el análisis se guiará por las siguientes hipótesis testables:

* **H1 (Viticultura):** El aumento de temperaturas y días de calor extremo en Marlborough y Hawke's Bay se correlacionará positivamente con la compresión de la cosecha y una mayor variabilidad en la producción de uva.
* **H2 (Lechería):** El aumento de "días de estrés por calor" en Waikato y Canterbury se correlacionará negativamente con la producción de leche por vaca.
* **H3 (Kiwis):** La disminución de "unidades de frío invernal" en Bay of Plenty se correlacionará negativamente con el rendimiento de las variedades de kiwi verde (Hayward).
* ## 4. Stack Tecnológico

* **Lenguaje:** Python
* **Análisis y Manipulación:** Pandas, NumPy, GeoPandas
* **Base de Datos:** SQLite (vía SQLAlchemy)
* **Visualización:** Plotly, Matplotlib, Seaborn
* **Dashboard Interactivo:** Streamlit
* **Control de Versiones:** Git y GitHub
* **Entorno Virtual:** venv / conda

## 5. Estructura del Repositorio

El proyecto está organizado de manera lógica para facilitar la navegación, el mantenimiento y la reproducibilidad.
/
├── data/
│   ├── raw/          # Archivos de datos originales sin procesar
│   └── processed/    # Base de datos limpia y archivos intermedios
├── notebooks/        # Cuadernos de Jupyter para exploración y análisis
├── src/              # Scripts de Python con funciones reutilizables
├── app/              # Código de la aplicación Streamlit
├── .gitignore
├── requirements.txt  # Lista de dependencias para la reproducibilidad
└── README.md         # Este mismo archivo, el documento central del proyecto

## 6. Fuentes de Datos

La adquisición de datos se planificó proactivamente para integrar información de múltiples agencias gubernamentales, un desafío clave del proyecto.

| Dataset | Fuente | Variables Clave | Formato/Acceso | Relevancia para la Hipótesis |
| :--- | :--- | :--- | :--- | :--- |
| **Clima Histórico** | NIWA DataHub | Temp. Max/Min Diaria, Precipitación | CSV (requiere registro) | Base para calcular métricas históricas como `heat_stress_days` y `winter_chill_units`. |
| **Proyecciones Climáticas**| NIWA / MfE Portal | Temp., Lluvia, Días de Calor >25°C bajo escenarios SSP | NetCDF o CSV | Núcleo del análisis de riesgo futuro. |
| **Producción Agrícola** | Stats NZ (Aotearoa Data Explorer) | Hectáreas de cultivo, producción total por región | CSV (vía ADE) o Excel | Variable dependiente para los modelos de correlación. |
| **Límites Regionales** | Stats NZ / LINZ | Geometrías poligonales de las regiones | Shapefile o GeoJSON | Esencial para la visualización geoespacial. |
## 6. Fuentes de Datos

La adquisición de datos se planificó proactivamente para integrar información de múltiples agencias gubernamentales, un desafío clave del proyecto.

| Dataset | Fuente | Variables Clave | Formato/Acceso | Relevancia para la Hipótesis |
| :--- | :--- | :--- | :--- | :--- |
| **Clima Histórico** | NIWA DataHub | Temp. Max/Min Diaria, Precipitación | CSV (requiere registro) | Base para calcular métricas históricas como `heat_stress_days` y `winter_chill_units`. |
| **Proyecciones Climáticas**| NIWA / MfE Portal | Temp., Lluvia, Días de Calor >25°C bajo escenarios SSP | NetCDF o CSV | Núcleo del análisis de riesgo futuro. |
| **Producción Agrícola** | Stats NZ (Aotearoa Data Explorer) | Hectáreas de cultivo, producción total por región | CSV (vía ADE) o Excel | Variable dependiente para los modelos de correlación. |
| **Límites Regionales** | Stats NZ / LINZ | Geometrías poligonales de las regiones | Shapefile o GeoJSON | Esencial para la visualización geoespacial. |

