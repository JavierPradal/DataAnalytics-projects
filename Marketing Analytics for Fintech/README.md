# 📊 Marketing Analytics for Fintech

## Descripción
Análisis completo de estrategias de marketing en el sector fintech, incluyendo métricas de rendimiento, insights del mercado y recomendaciones estratégicas.

## 📁 Contenidos

### 📄 Fintech_Report.pdf
Reporte ejecutivo con:
- **Análisis de Mercado** - Tendencias y oportunidades en fintech
- **Estrategias de Marketing Digital** - Canales y tácticas efectivas
- **Métricas y KPIs** - Indicadores de rendimiento clave
- **Visualizaciones** - Gráficos y dashboards de datos
- **Conclusiones y Recomendaciones** - Plan de acción

## 🖥️ Dashboard Interactivo

[#-dashboard-interactivo](#-dashboard-interactivo)

Además del reporte en PDF, el análisis está disponible como dashboard interactivo en Looker Studio, con filtros por campaña, mes, día, nivel educativo, edad y perfil laboral:

[📊 Ver Dashboard en Looker Studio](https://datastudio.google.com/reporting/eeafe9a0-1daf-474e-88b9-c984ca16f8dc)

## 📊 Visualizaciones del Reporte

### Página 1 - Portada y Resumen Ejecutivo
![Página 1](./page-1.png)

### Página 2 - Análisis de Mercado
![Página 2](./page-2.png)

### Página 3 - Estrategias y Métricas
![Página 3](./page-3.png)

### Página 4 - Conclusiones y Recomendaciones
![Página 4](./page-4.png)

## 🎯 Objetivos
- Evaluar el panorama del marketing en fintech
- Identificar oportunidades de crecimiento
- Proporcionar estrategias basadas en datos
- Optimizar ROI en campañas digitales

## 📊 Insights principales

- **Duración de la llamada como predictor clave**: los clientes que finalmente se suscribieron tuvieron una duración media de contacto de 9:13 min, frente a solo 3:40 min en los que no convirtieron — la duración de la conversación es la señal más fuerte de intención de compra.

- **Fatiga de campaña**: la tasa de conversión cae drásticamente con el número de contactos repetidos. Las primeras campañas alcanzan un 13,04% de conversión, mientras que las campañas de recontacto tardío caen por debajo del 5% (varias incluso al 0%). Esto sugiere que insistir sobre la misma audiencia tiene rendimientos decrecientes rápidos, y que los recursos deberían priorizarse en las primeras oleadas de contacto.

- **Perfil demográfico del cliente que convierte**: los clientes con estudios universitarios y el segmento de 17-32 años muestran las tasas de suscripción más altas, mientras que los perfiles con educación básica convierten notablemente menos.

- **Estacionalidad**: los meses de marzo, septiembre y diciembre concentran los picos de conversión, frente a un volumen mucho menor (aunque de mayor contacto total) en mayo, julio y agosto.

- **Modelo predictivo (XGBoost)**: se entrenó un modelo de clasificación para estimar la probabilidad de conversión por cliente, usando como variables principales duración de contacto, número de contactos previos, educación, edad y ocupación — pensado para priorizar a qué clientes contactar primero en futuras campañas.

- **Conversión global**: 11,27% sobre 41.162 clientes contactados, con un margen claro de mejora si se optimiza el timing y la segmentación de contacto en lugar de aplicar la misma estrategia a toda la base.

## 💡 Recomendaciones de negocio

- **Priorizar recursos en las primeras oleadas de contacto**: dado que las campañas iniciales convierten muy por encima de los recontactos tardíos (13% vs <5%), tiene más sentido invertir presupuesto y esfuerzo comercial en llegar a clientes nuevos que insistir repetidamente sobre la misma base de contacto.

- **Usar la duración de la llamada como señal temprana de calidad de lead**: si un contacto se está alargando por encima de la media, podría activarse como indicador en tiempo real para priorizar seguimiento inmediato o pasar la llamada a un agente senior.

- **Segmentar la estrategia de contacto por perfil demográfico**: enfocar campañas específicas hacia el segmento 17-32 años y clientes con estudios universitarios, que muestran mayor propensión a convertir, en lugar de aplicar el mismo guion y frecuencia de contacto a toda la base de clientes.

- **Aplicar el modelo predictivo como filtro previo a la campaña**: usar las probabilidades de conversión estimadas por el modelo XGBoost para priorizar la lista de contacto antes de lanzar una nueva oleada, en vez de contactar a toda la base por igual — reduciendo coste operativo y mejorando la tasa de conversión efectiva.

## 📈 Palabras Clave
`fintech` `marketing analytics` `digital marketing` `data analysis` `financial technology`

## 📦 Archivos del Proyecto
- **Modelo_XGBoost_FINAL.ipynb** - Modelo de machine learning para predicción
- **bank-additional_bank-additional-full.csv** - Dataset de análisis
- **Fintech_Report.pdf** - Reporte completo en PDF

## 🔎 Sobre Modelo_XGBoost_FINAL.ipynb
A continuación se añade una descripción práctica y reproducible del notebook `Modelo_XGBoost_FINAL.ipynb`, para que lectorxs y usuarixs puedan entender qué hace, cómo reproducirlo y qué resultados esperar.

### Objetivo del notebook
- Entrenar y evaluar un modelo XGBoost para predecir la variable objetivo presente en `bank-additional_bank-additional-full.csv` (por ejemplo, respuesta a una campaña o conversión), optimizando rendimiento y explicabilidad.

### Contenido y secciones principales
1. Carga de datos
   - Lectura del CSV `bank-additional_bank-additional-full.csv`.
   - Inspección inicial: dimensiones, tipos, valores faltantes.
2. Preprocesamiento
   - Limpieza de valores nulos y tratamiento de outliers cuando aplica.
   - Codificación de variables categóricas (One-Hot Encoding o Label Encoding según el caso).
   - Escalado/normalización de variables numéricas si es necesario.
   - Creación/selección de features: generación de variables temporales, agregados y transformaciones relevantes.
3. División de datos
   - Split train/test (p. ej. 80/20) con seed para reproducibilidad.
   - Opcional: validación cruzada (k-fold) o validación con TimeSeriesSplit si aplica.
4. Entrenamiento del modelo
   - Uso de XGBoost (xgboost.XGBClassifier / XGBRegressor según objetivo).
   - Búsqueda de hiperparámetros mediante GridSearchCV o RandomizedSearchCV (parámetros típicos: n_estimators, max_depth, learning_rate, subsample, colsample_bytree).
   - Entrenamiento final con los mejores hiperparámetros.
5. Evaluación
   - Métricas reportadas: ROC AUC, Accuracy, Precision, Recall, F1-score (para clasificación) — o RMSE/MAE/R2 para regresión.
   - Curvas ROC, matriz de confusión y reportes de clasificación.
6. Interpretabilidad
   - Importancia de features (feature_importances_ y/o SHAP values).
   - Visualizaciones de las características más relevantes y su impacto en la predicción.
7. Resultados y conclusiones
   - Resumen de desempeño del modelo.
   - Recomendaciones prácticas derivadas del modelo (p. ej. variables con mayor impacto en la conversión).
8. Exportar modelo
   - Guardado del modelo entrenado (p. ej. con joblib o pickle) para uso posterior en producción o scoring offline.

### Requisitos para ejecutar
- Python 3.8+ recomendado
- Dependencias principales (ejemplos):
  - pandas
  - numpy
  - scikit-learn
  - xgboost
  - shap (opcional, para interpretabilidad)
  - matplotlib / seaborn

Se recomienda crear un entorno virtual e instalar dependencias con `pip install -r requirements.txt` si existe, o instalar las librerías listadas.

### Cómo ejecutar
1. Clonar el repositorio y navegar a la carpeta del proyecto.
2. Asegurarse de tener `bank-additional_bank-additional-full.csv` en la misma carpeta o actualizar la ruta en el notebook.
3. Abrir `Modelo_XGBoost_FINAL.ipynb` en Jupyter Notebook o JupyterLab.
4. Ejecutar las celdas secuencialmente. Utilizar la celda con `random_state`/`seed` definida para obtener resultados reproducibles.

### Salidas esperadas
- Métricas de evaluación en conjunto de validación y test.
- Gráficos: curva ROC, matriz de confusión, importancias de features, gráficos SHAP (si se usa).
- Archivo de modelo exportado (p. ej. `modelo_xgboost.pkl`), si está incluida la celda de guardado.

### Notas y recomendaciones
- Documentar en el notebook las decisiones de preprocesamiento y la razón de elegir XGBoost.
- Si el dataset está desbalanceado, considerar técnicas como oversampling (SMOTE), undersampling o ajuste de `scale_pos_weight` en XGBoost.
- Para producción, serializar pipeline completo (preprocesamiento + modelo) y versionar el artefacto.
- Añadir pruebas rápidas o un script `predict.py` para scoring batch si se desea reutilizar el modelo fuera del notebook.

---

## 🔗 Acceso Rápido
[📥 Descargar Reporte](./Fintech_Report.pdf)

---
**Proyecto:** DataAnalytics-projects  
**Autor:** JavierPradal  
**Fecha:** 2026
