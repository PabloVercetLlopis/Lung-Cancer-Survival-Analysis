Análisis de Supervivencia en Pacientes con Cáncer de Pulmón

📄 Descripción del Proyecto:

Este proyecto se centra en realizar un análisis de supervivencia utilizando el dataset lung incluido en la biblioteca survival. El objetivo principal es identificar los factores que afectan la supervivencia en pacientes con cáncer avanzado de pulmón, empleando herramientas estadísticas como la estimación de Kaplan-Meier, pruebas de hipótesis y modelos de riesgos proporcionales de Cox.

🛠️ Requerimientos:

El análisis fue desarrollado en RStudio utilizando las siguientes bibliotecas:

tidyverse
ggplot2
kableExtra
survival
survminer
Asegúrate de tener R y estas bibliotecas instaladas antes de ejecutar los scripts.

📂 Estructura del Proyecto:

``` {r}
Lung-Cancer-Survival-Analysis/
├── analysis.Rmd                   # Archivo R Markdown con el análisis
├── lung_cancer_dataset.RData      # Dataset utilizado (incluido en R)
├── plots/                         # Gráficos generados durante el análisis
│   ├── survival_curves.png        # Curvas de supervivencia de Kaplan-Meier
│   ├── cox_diagnostics.png        # Gráficos de diagnóstico del modelo de Cox
├── README.md                      # Este archivo
├── results/                       # Resultados estadísticos
│   ├── summary_statistics.txt     # Estadísticas descriptivas
│   ├── cox_model_summary.txt      # Resumen del modelo de Cox
```

🚀 Pasos para Reproducir el Análisis:

Cargar el proyecto en RStudio: Abre el archivo analysis.Rmd.
Ejecutar los chunks de código: Sigue las secciones para reproducir las curvas de supervivencia, las pruebas estadísticas y los modelos de Cox.
Revisar los resultados:
Los gráficos generados se guardan en la carpeta plots/.
Las estadísticas resumidas se encuentran en la carpeta results/.

🧪 Metodología:

Análisis Realizado:
Exploración de datos:
Resumen descriptivo de las variables relevantes en el dataset.
Curvas de Kaplan-Meier:
Estimación de supervivencia estratificada por género.
Análisis de diferencias con pruebas de hipótesis.
Modelos de Cox:
Análisis univariado para evaluar el impacto de diferentes covariables.
Modelo multivariable ajustado con validación de supuestos.
Validación:
Comprobación de riesgos proporcionales y diagnóstico del modelo.
Principales Resultados:
La mediana de supervivencia es significativamente mayor en mujeres (426 días) que en hombres (270 días).
Los resultados de los modelos de Cox muestran que:
Ser mujer está asociado con un menor riesgo de muerte (HR = 0.58, p < 0.05).
Un mayor ph.ecog incrementa significativamente el riesgo de muerte (HR = 1.58, p < 0.05).
La edad no es significativa en el modelo multivariable (p > 0.05).

📈 Conclusiones:

El análisis confirma que el género y el ph.ecog son factores significativos en la supervivencia de los pacientes. Además, la validación del modelo indica que los supuestos de riesgos proporcionales se cumplen, validando el uso del modelo de Cox en este estudio.

🖊️ Autor:

Pablo Vercet
Proyecto desarrollado como parte de un análisis de supervivencia en RStudio.
