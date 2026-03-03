💳 Detección de Fraude con Machine Learning: Optimización para Reducción de Pérdidas Financieras
📍 Caso de Estudio – NovaSur Analytics S.A. (CABA, Buenos Aires)

Proyecto para el área de Prevención de Fraude de NovaSur Analytics S.A., enfocado en optimizar modelos de clasificación desbalanceados mediante una evaluación basada en impacto económico real.

❓ Problema de Negocio

NovaSur Analytics enfrentaba pérdidas significativas derivadas de transacciones fraudulentas no detectadas.

El modelo tradicional priorizaba métricas como accuracy, lo que generaba una falsa sensación de desempeño en un contexto de datos desbalanceados (10.9% de fraude).

Este proyecto responde a preguntas clave:

¿Es suficiente maximizar accuracy en un problema de fraude?

¿Cómo afecta el desbalance de clases al rendimiento real?

¿Cómo seleccionar el umbral óptimo cuando los falsos negativos son mucho más costosos?

¿Se puede optimizar un modelo directamente en función del impacto financiero?

🎯 Objetivos del Proyecto

Analizar el comportamiento del fraude en un dataset desbalanceado.

Construir un modelo baseline y evaluar sus limitaciones.

Aplicar técnicas de balanceo (SMOTE) evitando data leakage.

Comparar múltiples modelos de Machine Learning.

Optimizar el umbral de decisión en función de costos financieros.

Cuantificar el impacto económico del modelo optimizado.

Traducir métricas técnicas a resultados estratégicos de negocio.

🧪 Metodología
1️⃣ Análisis Exploratorio de Datos (EDA)

Evaluación de desbalance (10.9% fraude)

Análisis geográfico (Argentina, Brasil, Chile)

Identificación de patrones conductuales

2️⃣ Modelo Baseline

Logistic Regression sin balanceo

Accuracy: 89%

Recall fraude: 17%

Identificación de alto riesgo financiero por falsos negativos

3️⃣ Manejo del Desbalance

Aplicación de SMOTE exclusivamente sobre el set de entrenamiento

Prevención de data leakage

Mejora significativa del recall

4️⃣ Modelos Avanzados

Random Forest

XGBoost

Validación cruzada usando PR-AUC

5️⃣ Optimización del Umbral

Simulación de costos:

Falso Negativo (FN): $500

Falso Positivo (FP): $10

Selección del threshold basado en mínimo costo total y trade-off precision–recall.

💰 Resultado de Negocio
Modelo	Costo Estimado
Baseline	$136,000
Modelo Optimizado (XGBoost)	$28,380
➡ Reducción superior al 60% en pérdidas estimadas.

El modelo optimizado demuestra que ajustar el umbral en función del impacto económico es más relevante que maximizar accuracy.

📊 Métricas Clave

ROC-AUC: 0.835

PR-AUC Test: 0.308

Recall optimizado > 80% en ciertos thresholds

Reducción significativa de falsos negativos

🏆 Diferencial del Proyecto

Este proyecto destaca por:

✔ Aplicar correctamente técnicas para datasets desbalanceados
✔ Evitar data leakage
✔ Priorizar PR-AUC sobre accuracy
✔ Optimizar decisiones basadas en impacto financiero
✔ Traducir métricas técnicas en resultados estratégicos

🛠️ Tecnologías Utilizadas

Python

Pandas

NumPy

Scikit-learn

Imbalanced-learn (SMOTE)

XGBoost

Plotly

Jupyter Notebook

📌 Conclusión Ejecutiva

La optimización del modelo de detección de fraude basada en impacto económico permitió reducir significativamente las pérdidas estimadas, demostrando que la correcta selección del umbral y la evaluación con métricas adecuadas pueden generar mejoras financieras sustanciales.
