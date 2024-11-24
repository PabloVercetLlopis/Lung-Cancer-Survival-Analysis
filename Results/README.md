# Resultados del Proyecto

Este directorio contiene las visualizaciones y resultados generados en el análisis de supervivencia. 

## Contenido
- `curva de supervivencia por genero.PNG`: Gráfico de curvas de Kaplan-Meier, mostrando la probabilidad de supervivencia por género, siendo sex1= Hombres y sex2= Mujeres.
- prueba de hipotesis para comparar 2 o + funciones de supervivencia.PNG: Es una prueba de hipótesis donde se observa que el p-valor<0.05, por lo que se concluye que la supervivencia difere significativamente por género. 
- `Regresion de cox multivariable.PNG`: Muestra que los resultados generales (p.valor<0.05), por lo que el modelo es significativo. 
      Sex y ph.ecog son estadisticamente significativas 
      Age al tener un pvalor >0.05 no es significativa. 
      HR de sex con 0.58 y p-valor<0.05 muestra una fuerte relacion entre la variable y el decrecimiento de muerte
      HR de ph.ecog con 1.58 y p-valor<0.05 muestra una fuerte relacion entre la variable y el incremento de muerte
      HR de age con 1.01 y p.valor>0.05 muestra que no hay relacion entre la variable y el riesgo de muerte
- `Validacion de supuestos.PNG`: Se observa que todos los p-valores son >0.05 por lo que la prueba no es estadisticamente signifcativa para las covariables ni como para el modelo global. Por lo tanto, se pueden asumir los riesgos proporcionales. Bien hecho el utilizar Cox.
- `Validacion de supuestos grafica.PNG`: Gráfico de la validacion de supuestos.
- `grafica observaciones influyentes.PNG`: Los valores positivos corresponden a pacientes que mueren pronto comparado con el tiempo de supervivencia estimado; mientras que valores negativos corresponden a pacientes que viven mucho comparado con el tiempo de supervivencia estimado. Los valores lejanos del 0 son outliers, que dificultan la prediccion del modelo. 


Todos los gráficos fueron generados con el código contenido en el archivo `Código fuente`.
