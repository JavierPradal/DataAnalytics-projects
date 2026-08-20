# Idealista Real Estate Analysis 🏠

## Overview

Análisis exhaustivo del mercado inmobiliario español utilizando datos de **Idealista**, la plataforma de referencia en compraventa de viviendas en España. Este proyecto proporciona insights detallados sobre precios, tendencias del mercado, ubicaciones y factores que influyen en la valoración de propiedades en Madrid.

**Dataset:** Análisis de miles de propiedades en Madrid con múltiples variables de caracterización (precios, superficie, ubicación, características constructivas, etc.)

---

## 🎯 Objetivos Principales

Este proyecto analiza los siguientes aspectos del mercado inmobiliario:

- 📍 **Análisis Geográfico:** Identificar distritos y barrios con precios más altos y más bajos
- 💰 **Valoración de Propiedades:** Entender qué factores influyen en el precio (m², habitaciones, año construcción, etc.)
- 📊 **Tendencias del Mercado:** Detectar patrones y comportamientos generales
- 🔍 **Segmentación:** Clasificar propiedades por tipología, rango de precio y características
- 📈 **Correlaciones:** Identificar relaciones entre variables y el precio final
- 🏘️ **Distribuciones:** Analizar cómo se distribuyen las propiedades por tipo, zona y precio

---

## 📁 Contenido del Proyecto

```
Idealista Analysis/
├── BBDD_Javier_Pradal.ipynb          # Notebook completo con análisis
├── madrid_dataset.csv                 # Dataset con ~16 MB de propiedades
├── idealista.db                       # Base de datos SQLite procesada
└── README.md                          # Este archivo
```

---

## 📦 Datos Disponibles

### Dataset Principal: `madrid_dataset.csv`
- **Tamaño:** ~16 MB
- **Registros:** Miles de propiedades en Madrid
- **Tipo de análisis:** Real estate (compraventa, alquiler, etc.)

### Variables Clave:
- `precio` - Precio de la propiedad
- `m2` - Superficie en metros cuadrados
- `habitaciones` - Número de habitaciones
- `baños` - Número de baños
- `año_construccion` - Año de construcción
- `distrito` / `barrio` - Ubicación geográfica
- `tipo_propiedad` - Clasificación (piso, chalet, etc.)
- `planta` - Planta en la que se encuentra
- `orientacion` - Orientación de la vivienda
- Y múltiples variables adicionales de caracterización

### Base de Datos: `idealista.db`
- Base de datos SQLite con datos procesados
- Tablas optimizadas para consultas rápidas
- Ideal para análisis avanzados y reportes

---

## 🔍 Preguntas Clave que Responde

- ¿Cuáles son los barrios más caros y más económicos de Madrid?
- ¿Cómo varía el precio según la superficie, número de habitaciones y año de construcción?
- ¿Qué tipo de propiedades dominan el mercado?
- ¿Existen diferencias significativas entre distritos?
- ¿Cuál es la relación entre las características de una propiedad y su precio?
- ¿Cuáles son los factores más determinantes en la valoración?

---

## 📊 Análisis Incluido en el Notebook

El notebook `BBDD_Javier_Pradal.ipynb` contiene:

### 1. **Exploración Inicial**
- Carga y descripción del dataset
- Revisión de estructura, tipos de datos y valores faltantes
- Estadísticas descriptivas básicas

### 2. **Limpieza de Datos**
- Tratamiento de valores atípicos y faltantes
- Validación de datos
- Transformaciones necesarias

### 3. **Análisis Exploratorio (EDA)**
- Distribuciones de precios y variables clave
- Análisis por zonas geográficas
- Comparativas entre tipos de propiedades
- Relaciones entre variables

### 4. **Visualización de Datos**
- Gráficos de distribución (histogramas, densidades)
- Comparaciones geográficas
- Análisis de correlaciones
- Gráficos comparativos por segmentos

### 5. **Insights y Conclusiones**
- Identificación de patrones clave
- Oportunidades del mercado
- Recomendaciones basadas en datos

---

## 🛠️ Requisitos Técnicos

### Versión de Python
- Python 3.8 o superior

### Librerías Principales
```
pandas          # Manipulación de datos
numpy           # Operaciones numéricas
matplotlib      # Visualizaciones estáticas
seaborn         # Visualizaciones estadísticas
sqlite3         # Manejo de base de datos
jupyter         # Entorno interactivo
scikit-learn    # Machine Learning (opcional)
```

### Instalación
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

---

## 🚀 Cómo Ejecutar el Análisis

### Opción 1: Ver en GitHub
1. Abre el notebook directamente: [BBDD_Javier_Pradal.ipynb](./BBDD_Javier_Pradal.ipynb)
2. GitHub renderiza automáticamente el notebook con todos los gráficos y resultados

### Opción 2: Ejecutar Localmente

```bash
# 1. Clonar el repositorio
git clone https://github.com/JavierPradal/DataAnalytics-projects.git
cd "Idealista Analysis"

# 2. Crear entorno virtual (opcional pero recomendado)
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate

# 3. Instalar dependencias
pip install pandas numpy matplotlib seaborn jupyter

# 4. Iniciar Jupyter
jupyter notebook BBDD_Javier_Pradal.ipynb
# o
jupyter lab BBDD_Javier_Pradal.ipynb

# 5. Ejecutar las celdas en orden
```

---

## 💡 Casos de Uso

Este análisis es útil para:

- 🏠 **Compradores:** Entender precios de mercado por zona y características
- 🏘️ **Vendedores:** Valorar sus propiedades de manera realista
- 📈 **Inversores:** Identificar zonas con potencial de inversión
- 📊 **Analistas:** Estudiar tendencias del mercado inmobiliario madrileño
- 🎓 **Estudiantes:** Aprender análisis de datos en contextos reales
- 🔍 **Agentes Inmobiliarios:** Acceder a análisis de mercado competitivo

---

## 📈 Tecnologías Utilizadas

- **Python 3.8+** - Lenguaje principal
- **Jupyter Notebook** - Entorno de análisis interactivo
- **Pandas** - Manipulación y análisis de datos
- **Matplotlib & Seaborn** - Visualización de datos
- **NumPy** - Computación numérica
- **SQLite** - Base de datos

---

## 📝 Notas Importantes

⚠️ **Sobre los Datos:**
- Los datos provienen de Idealista, plataforma de referencia en España
- Pueden contener valores faltantes o datos atípicos que se tratan en el análisis
- Se recomienda validar los resultados con expertos del sector

🔒 **Privacidad:**
- El dataset no contiene información personal identificable
- Uso exclusivo con propósitos educativos y profesionales

📅 **Temporalidad:**
- Los datos corresponden a un período específico
- Pueden actualizarse descargando nuevos datos de Idealista

---

## 🤝 Contribuciones

Si quieres mejorar este análisis:

1. Abre un **issue** describiendo tu propuesta
2. Crea una rama con nombre descriptivo
3. Envía un **pull request** con cambios claros

**Sugerencias de mejora:**
- Análisis adicionales (predicción de precios con ML)
- Nuevas visualizaciones
- Optimización del código
- Ampliación a otras ciudades españolas

---

## 📧 Contacto

**Javier Pradal**  
🔗 [GitHub](https://github.com/JavierPradal)  
📍 Madrid, España

Para preguntas o sugerencias, abre un issue en el repositorio.

---

## 📄 Licencia

**MIT License** - Este proyecto está disponible bajo licencia MIT.

---

**Última actualización:** Agosto 2026  
**Estado:** ✅ Completo y funcional
