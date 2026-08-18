# Amazon Charback Analysis

Este repositorio contiene el análisis exploratorio y modelos relacionados con los "Amazon Chargeback" (nota: el nombre de la carpeta original es "Amazon Charback Analysis"). El objetivo es estudiar patrones de cobros/contracargos y comportamientos relacionados para extraer insights y construir modelos predictivos.

## Contenido

- Notebooks/:
  - Todos los notebooks Jupyter usados para la carga, limpieza, análisis exploratorio, visualización y modelado.
- data/ (si está incluida):
  - Archivos CSV/Parquet usados en el análisis (si no están, se indican las instrucciones para obtenerlos).
- outputs/:
  - Gráficos y reportes generados por los notebooks.

> Nota: Los archivos de datos sensibles no deberían subirse al repositorio; en su lugar, incluir instrucciones para descargar o preparar los datos.

## Requisitos

- Python 3.9+ recomendado
- Jupyter Notebook o JupyterLab
- Paquetes principales (instalar con pip o conda):
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn
  - plotly (opcional, para visualizaciones interactivas)
  - seaborn
  - jupyter

Ejemplo usando pip:

pip install -r requirements.txt

Si no existe `requirements.txt`, se puede crear con:

pip install pandas numpy matplotlib seaborn scikit-learn plotly jupyter

## Estructura sugerida de notebooks

1. 00_data_load_and_cleaning.ipynb - carga y limpieza de datos
2. 01_exploratory_analysis.ipynb - análisis exploratorio y visualizaciones
3. 02_feature_engineering.ipynb - creación de variables para modelos
4. 03_modeling.ipynb - entrenamiento y evaluación de modelos
5. 04_reporting_and_conclusions.ipynb - reportes finales y conclusiones

Adapte los nombres según los notebooks presentes.

## Cómo ejecutar

1. Clona el repositorio:

git clone https://github.com/JavierPradal/DataAnalytics-projects.git
cd "Amazon Charback Analysis"

2. Crea y activa un entorno virtual (opcional pero recomendado):

python -m venv venv
source venv/bin/activate  # Linux / macOS
venv\Scripts\activate     # Windows

3. Instala dependencias:

pip install -r requirements.txt

4. Lanza Jupyter Lab / Notebook:

jupyter lab
# o
jupyter notebook

5. Abre los notebooks listados y ejecuta las celdas en orden.

## Notas sobre datos

- Si los datos no están incluidos, agregue un script `scripts/download_data.sh` o instrucciones en un notebook para reconstruir/descargar el dataset desde la fuente original.
- Mantenga archivos con credenciales fuera del repositorio. Use variables de entorno o un archivo `.env` ignorado por Git.

## Resultados esperados

- Visualizaciones que identifiquen patrones en chargebacks por producto, región, método de pago y tiempo.
- Un pipeline simple que permita predecir probabilidad de chargeback por transacción.
- Métricas de evaluación (ROC-AUC, precision/recall, F1) y un análisis de las características más importantes.

## Contribuciones

Si quieres contribuir:
- Abre un issue describiendo la propuesta.
- Crea una rama con un nombre descriptivo.
- Envía un pull request con cambios claros y notebooks ejecutados.

## Licencia

Añade una licencia apropiada (por ejemplo MIT) si deseas permitir contribuciones y uso público.

## Contacto

Javier Pradal - perfil de GitHub: https://github.com/JavierPradal

