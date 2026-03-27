Este README está diseñado para destacar tus habilidades en **Análisis de Datos, Estadística y Toma de Decisiones**. Sigue esta estructura para que tu perfil de GitHub se vea profesional.

-----

# 📊 Análisis de Experimento A/B: Optimización de Landing Page

Este proyecto consiste en un análisis estadístico riguroso de un **Experimento A/B** realizado sobre dos versiones de una página de inicio (Landing Page). El objetivo principal es determinar, mediante datos, qué versión maximiza el valor para el negocio en términos de **conversión** y **gasto promedio por usuario**.

## 🎯 Objetivos del Proyecto

  * Validar la integridad y calidad de los datos del experimento.
  * Comparar el **Gasto Promedio** entre la versión A y B (Métrica de Valor).
  * Evaluar la **Tasa de Conversión (CR)** mediante pruebas de significancia (Métrica de Éxito).
  * Analizar el impacto de segmentaciones como **fuente de tráfico** y **tipo de usuario**.
  * Proporcionar una recomendación final basada en evidencia estadística.

-----

## 🛠️ Stack Tecnológico

  * **Lenguaje:** Python 3.x
  * **Manipulación de Datos:** `Pandas`, `Numpy`
  * **Visualización:** `Matplotlib`, `Seaborn`
  * **Estadística:** `SciPy` (Mann-Whitney U), `Statsmodels` (Z-test, Chi-squared)

-----

## 📈 Metodología y Pruebas Estadísticas

El análisis se dividió en etapas clave para asegurar la validez de las conclusiones:

### 1\. Exploración de Datos (EDA)

Se analizaron 40,000 registros balanceados (\~50/50 por variante). Se confirmó que el tráfico es mayoritariamente **Mobile (62%)** y proveniente de fuentes **Orgánicas (45%)**.

### 2\. Análisis de Gasto (Prueba U de Mann-Whitney)

Debido a que el gasto no sigue una distribución normal y presenta valores atípicos, se utilizó una prueba no paramétrica.

  * **Resultado:** Se encontró una diferencia estadísticamente significativa ($p < 0.05$). La variante B genera un comportamiento de compra distinto y superior.

### 3\. Análisis de Conversión (Prueba Z de Proporciones)

Comparamos si el incremento en la tasa de conversión de la página B fue producto del azar o del diseño.

  * **Resultado:** Con un valor $Z$ de $-9.67$, se rechaza la hipótesis nula. La Landing B es significativamente más efectiva para convertir usuarios.

### 4\. Segmentación por Fuente y Usuario (Chi-cuadrado)

  * **Tráfico:** Existe una relación significativa entre el origen del usuario y su probabilidad de convertir.
  * **Tipo de Usuario:** No se encontró diferencia significativa entre usuarios nuevos y recurrentes, lo que indica que la página funciona igual de bien para ambos perfiles.

-----

## 🚀 Conclusiones de Negocio

1.  **Landing Page B.** Supera a la versión A tanto en volumen de conversiones como en el valor monetario de las mismas.
2.  **Significancia:** Los resultados son altamente confiables ($p \approx 0$).
3.  **Recomendación:** Implementar la versión B de forma para nuevos reclutamientos y compras sencillas y optimizar las campañas de las fuentes de tráfico con mayor CR (Ads y Email).

-----

## 📂 Estructura del Repositorio

  * `notebook.ipynb`: Jupyter Notebook con todo el flujo de análisis, código y gráficas.
  * `/datasets/landing_experiment.csv`: Datos en bruto del experimento.
  * `images/`: Exportación de las visualizaciones principales.

-----

## 👤 Autor

**Liz Aguirre, como parte del proyecto spring 9. Data ANalyst en proceso.

-----

### ¿Cómo usar este repositorio?

1.  Clona el proyecto: `git clone [https://github.com/tu-usuario/ab-test-landing.git](https://github.com/tu-usuario/ab-test-landing.git)](https://github.com/eeac0022-svg/Analisis-de-Experimento-A-B-Optimizacion-de-Landing-Page/new/main?readme=1)`
2.  Instala las dependencias: `pip install -r requirements.txt`
3.  Ejecuta el notebook para replicar los resultados.
