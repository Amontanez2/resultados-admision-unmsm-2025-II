# 📊 Resultados de Admisión UNMSM 2025-II

Este proyecto presenta un análisis visual interactivo de los resultados del proceso de admisión 2025-II de la **Universidad Nacional Mayor de San Marcos (UNMSM)**. La visualización fue desarrollada en **Power BI**, integrando diversas fuentes de datos en un solo informe dinámico.

---

## 🧠 Objetivo

Brindar una vista clara y estructurada de los resultados de admisión mediante dashboards intuitivos que faciliten la comprensión del rendimiento de los postulantes según:

- Escuela profesional  
- Área académica  
- Puntaje obtenido  
- Ubicación geográfica  
- Condición del postulante (ingresante, ausente, etc.)

---

🔍 Métricas destacadas

✅ Total de postulantes e ingresantes

📍 Postulantes por departamento de procedencia

🎯 Puntaje promedio de los ingresantes

🧾 Vacantes alcanzadas por carrera

❌ Número de ausentes

📊 Distribución por áreas académicas (A, B, C, D, E)

---

🛠️ Tecnologías utilizadas

- Python para la automatización de extracción de datos vía web scraping

- Power BI para la visualización y análisis de datos

- Transformación de datos con Power Query

- Cálculos mediante medidas DAX

- Datos extraídos desde archivos CSV por escuela profesional

## Vista Previa del Dashboard
![Admision Dashboard](https://github.com/Amontanez2/resultados-admision-unmsm-2025-II/blob/main/ResultadosAdmisionUNMSM2025.PNG?raw=true)

---
![Admision Dashboard](https://github.com/Amontanez2/resultados-admision-unmsm-2025-II/blob/main/ResultadosAdmisionUNMSM2025-1.PNG?raw=true)



# 🧱 Modelado de Datos

El modelo de datos fue diseñado bajo una estructura en estrella, teniendo como tabla de hechos principal a Resultados_Admision, la cual contiene los registros detallados de cada postulante, incluyendo su escuela profesional, puntaje, mérito y condición. Esta tabla se relaciona con diversas dimensiones para enriquecer el análisis:

- Dim_Escuela_Profesional: vincula cada postulante con su escuela y área académica.

- Dim_Estudiantes: permite identificar de forma única a cada postulante.

- Dim_Ubicacion: asocia la ubicación geográfica de los postulantes, clave para el análisis por departamentos.

Otras tablas como Datos_Adicionales o AREAS DE PROVINCIA se utilizaron como soporte durante el proceso de depuración y validación.

Gracias a este diseño relacional y limpio, se logró un análisis eficiente y dinámico en Power BI, facilitando la creación de medidas DAX para métricas clave como vacantes, puntajes promedio, ingresantes y ausentes.

📌 A continuación se muestra una imagen del modelo de datos implementado:

![Admision Dashboard](https://github.com/Amontanez2/resultados-admision-unmsm-2025-II/blob/main/modelado%20de%20datos.PNG?raw=true)

