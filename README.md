# Proyecto Olist – Análisis de Factores Logísticos y Satisfacción del Cliente

## Objetivo

Este proyecto tiene como propósito responder la siguiente pregunta de negocio:

**¿Qué factores logísticos diferencian los pedidos con alta y baja satisfacción del cliente en Olist?**

Adicionalmente, se aborda una segunda pregunta complementaria:

**¿Cuál es el impacto esperado de la tardanza en escenarios futuros bajo distintos perfiles de satisfacción?**

---

## Enfoque del análisis

Se construyó una base analítica integrando información de pedidos, reseñas, costos y geolocalización, con el fin de conectar el desempeño logístico con la percepción del cliente.

El análisis se desarrolló bajo un enfoque cuantitativo, utilizando técnicas estadísticas para modelar, segmentar y proyectar el comportamiento de los pedidos.

---

## Metodologías aplicadas

* Análisis exploratorio de datos (EDA)
  Identificación de patrones en tiempos de entrega, retrasos y niveles de satisfacción.

* Estimación por Máxima Verosimilitud (MLE)
  Comparación de distribuciones Normal y Log-Normal mediante AIC y BIC para modelar el tiempo de entrega.

* Inferencia Bayesiana
  Estimación de la probabilidad de tardanza condicionada al nivel de satisfacción, utilizando un prior Beta y una verosimilitud Binomial.

* Simulación Monte Carlo
  Proyección del impacto de la tardanza en escenarios futuros, cuantificando el riesgo operativo.

* Clustering (K-Means)
  Segmentación de pedidos en grupos logísticos diferenciados y validación mediante métricas como índice de silueta, Davies-Bouldin y Calinski-Harabasz.

---

## Principales hallazgos

* La tardanza es el factor que más diferencia la satisfacción del cliente.
* La probabilidad de que un pedido llegue tarde pasa de aproximadamente 3,5% en alta satisfacción a cerca del 25% en baja satisfacción.
* En escenarios futuros, esto representa más de 2.100 pedidos tardíos adicionales por cada 10.000 pedidos.
* Se identificaron dos segmentos logísticos: uno eficiente y otro problemático, con diferencias significativas en tiempo de entrega, retraso y distancia.

---

## Recomendaciones

* Reducir la tasa de tardanza como principal indicador operativo.
* Intervenir pedidos de larga distancia, donde se concentran los mayores tiempos y retrasos.
* Implementar sistemas de alerta temprana basados en probabilidad de tardanza.

---

## Estructura del repositorio

* Analisis_Olist_Logistica_Satisfaccion.ipynb: Notebook principal con el desarrollo completo del análisis.
* data/ (opcional): Archivos de datos si se incluyen localmente.

---

## Dataset

Fuente:
[https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

---

## Nota

Este proyecto fue desarrollado con fines académicos, aplicando técnicas de estadística avanzada para generar hallazgos accionables en un contexto de negocio.

---

## Conclusión

El principal factor logístico que diferencia los pedidos con alta y baja satisfacción en Olist es la tardanza, y es un factor que se puede medir, anticipar y gestionar.
