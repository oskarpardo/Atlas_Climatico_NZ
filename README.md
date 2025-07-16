# 📈 Atlas de Adaptación Agro-Climática de Nueva Zelanda para 2050

![Python](https://img.shields.io/badge/python-3.x-blue.svg) ![Pandas](https://img.shields.io/badge/pandas-2.x-blue.svg) ![NumPy](https://img.shields.io/badge/numpy-1.2x-blue.svg) ![Streamlit](https://img.shields.io/badge/streamlit-1.x-orange.svg) ![Plotly](https://img.shields.io/badge/plotly-5.x-orange.svg) ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

**Un proyecto de análisis de datos de ciclo completo para evaluar el riesgo climático y modelar estrategias de adaptación en las industrias primarias clave de Nueva Zelanda.**

---

### ➡️ [Ver Dashboard Interactivo en Vivo](http://URL_DE_TU_APP_CUANDO_ESTE_LISTA.streamlit.app)

*Aquí se insertará una GIF animada del dashboard final en acción para una demostración visual inmediata.*

---

## 1. Visión del Proyecto y Propuesta de Valor

[cite_start]Este proyecto simula un encargo de consultoría estratégica de alto nivel, diseñado para ir más allá del análisis de datos convencional[cite: 3]. [cite_start]El objetivo es construir un prototipo de **Herramienta de Evaluación de Riesgo Climático**[cite: 20]. [cite_start]La propuesta de valor es demostrar la capacidad de transformar datos dispares y complejos en una herramienta interactiva que facilita la toma de decisiones estratégicas a largo plazo[cite: 5, 40]. [cite_start]El resultado final no solo presenta hallazgos, sino que ofrece una solución que un stakeholder, como un viticultor o un planificador gubernamental, puede utilizar para explorar escenarios y planificar la adaptación[cite: 40, 262].

## 2. El Problema de Negocio

[cite_start]Las industrias primarias son la columna vertebral de la economía de exportación de Nueva Zelanda, definiendo la identidad productiva del país[cite: 7, 9]. [cite_start]Sin embargo, enfrentan una amenaza tangible y creciente por el cambio climático[cite: 10]. Este proyecto aborda los siguientes riesgos específicos y medibles:

* [cite_start]**Viticultura:** El calentamiento global está causando una "compresión de la cosecha", acelerando la maduración de la uva, lo que afecta su calidad y crea cuellos de botella logísticos[cite: 12].
* [cite_start]**Kiwis:** El aumento de las temperaturas invernales amenaza con la "pérdida de frío invernal", un requisito de horas a baja temperatura que las variedades de kiwi como Hayward necesitan para una brotación y cosecha abundantes[cite: 13, 14]. [cite_start]Esto pone en riesgo la viabilidad del cultivo en regiones clave como Bay of Plenty[cite: 15].
* [cite_start]**Lechería:** El incremento de "días de estrés por calor" (temperaturas > 25°C) puede reducir la ingesta de alimento del ganado, disminuir la producción de leche y afectar la salud general de los animales[cite: 16].

## 3. Hipótesis de Investigación

[cite_start]Para abordar este problema, el análisis se guiará por las siguientes hipótesis testables[cite: 48, 49]:

* [cite_start]**H1 (Viticultura):** El aumento de temperaturas y días de calor extremo en Marlborough y Hawke's Bay se correlacionará positivamente con la compresión de la cosecha y una mayor variabilidad en la producción de uva[cite: 51].
* [cite_start]**H2 (Lechería):** El aumento de "días de estrés por calor" en Waikato y Canterbury se correlacionará negativamente con la producción de leche por vaca[cite: 52].
* [cite_start]**H3 (Kiwis):** La disminución de "unidades de frío invernal" en Bay of Plenty se correlacionará negativamente con el rendimiento de las variedades de kiwi verde (Hayward)[cite: 53].

## 4. Stack Tecnológico

* **Lenguaje:** Python
* **Análisis y Manipulación:** Pandas, NumPy, GeoPandas
* **Base de Datos:** SQLite (vía SQLAlchemy)
* **Visualización:** Plotly, Matplotlib, Seaborn
* **Dashboard Interactivo:** Streamlit
* **Control de Versiones:** Git y GitHub
* [cite_start]**Entorno Virtual:** venv / conda [cite: 65]

## 5. Fuentes de Datos

[cite_start]La adquisición de datos se planificó proactivamente para integrar información de múltiples agencias gubernamentales, un desafío clave del proyecto[cite: 86].

| Dataset | Fuente | Variables Clave | Formato/Acceso | Relevancia para la Hipótesis |
| :--- | :--- | :--- | :--- | :--- |
| **Clima Histórico** | NIWA DataHub | Temp. Max/Min Diaria, Precipitación | CSV (requiere registro) | Base para calcular métricas históricas como `heat_stress_days`, `winter_chill_units`. |
| **Proyecciones Climáticas**| NIWA / MfE Portal | Temp., Lluvia, etc. bajo escenarios SSP | NetCDF o CSV | Núcleo del análisis de riesgo futuro. |
| **Producción Agrícola** | Stats NZ (Aotearoa Data Explorer) | Hectáreas de cultivo, producción total por región | CSV (vía ADE) o Excel | Variable dependiente para los modelos de correlación. |
| **Límites Regionales** | Stats NZ / LINZ | Geometrías poligonales de las regiones | Shapefile o GeoJSON | Esencial para la visualización geoespacial. |

## 6. Metodología y Fases del Proyecto

*Esta sección se rellenará a medida que avances. Será un resumen de los pasos clave en cada fase.*
* **Fase 1: Planificación y Diseño:** Definición de objetivos, hipótesis y plan de adquisición de datos.
* **Fase 2: Adquisición e Ingeniería de Datos:** Proceso de ETL (Extracción, Transformación, Carga), limpieza, unión y creación de características.
* **Fase 3: Modelado y Análisis Exploratorio:** Visualización, análisis de correlación y modelado de escenarios.
* **Fase 4: Comunicación y Despliegue:** Construcción y despliegue del dashboard interactivo con Streamlit.

## 7. Hallazgos Clave y Conclusiones

*Esta sección la rellenarás al final del proyecto. Será un resumen de tus descubrimientos más importantes y las respuestas a tus hipótesis.*

## 8. Instalación y Uso

*Aquí explicarás cómo otra persona puede clonar tu repositorio, instalar las dependencias con `pip install -r requirements.txt` y ejecutar tu análisis y aplicación.*

## 9. Licencia

Este proyecto está bajo la Licencia MIT.
