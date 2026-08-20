# 🏠 Análisis de Alojamientos Airbnb en Madrid

**📥 Descargar Presentación (PDF):**  
https://github.com/JavierPradal/DataAnalytics-projects/blob/main/Airbnb%20Analysis%20in%20Madrid/presentacio%CC%81n_analisis_airbnb_madrid.pdf

> Un análisis exhaustivo del mercado de alojamientos de Airbnb en Madrid, explorando patrones de precios, distribución geográfica, tipos de alojamiento y factores que influyen en la demanda.

## 📋 Tabla de Contenidos

- [Descripción General](#descripción-general)
- [Objetivo del Análisis](#objetivo-del-análisis)
- [Estructura del Proyecto](#estructura-del-proyecto)
- [Metodología](#metodología)
- [Datos](#datos)
- [Análisis Realizados](#análisis-realizados)
- [Hallazgos Clave](#hallazgos-clave)
- [Tecnologías Utilizadas](#tecnologías-utilizadas)
- [Cómo Usar Este Proyecto](#cómo-usar-este-proyecto)
- [Archivos del Proyecto](#archivos-del-proyecto)

---

## 📊 Descripción General

Este proyecto realiza un análisis completo del mercado de alojamientos en Airbnb dentro de Madrid, utilizando técnicas de análisis exploratorio de datos (EDA), visualización de datos y análisis estadístico avanzado.

### Aspectos Analizados:

- 💰 **Distribución de precios** por tipos de alojamiento, barrios y características
- 🗺️ **Ubicación geográfica** de los alojamientos y su impacto en los precios
- ⭐ **Valoraciones y satisfacción** de los clientes
- 🛏️ **Tipos y características** de los alojamientos más demandados
- 📈 **Tendencias del mercado** y oportunidades de negocio

---

## 🎯 Objetivo del Análisis

El análisis busca proporcionar **insights accionables** para:

- **Hosts (Propietarios)**: Optimizar precios y características de sus alojamientos
- **Inversores**: Identificar oportunidades rentables en el mercado madrileño
- **Plataforma Airbnb**: Entender comportamientos del mercado local
- **Turistas**: Comparar opciones de alojamiento según presupuesto y preferencias

**Preguntas Clave Respondidas:**
- ¿Cuáles son los barrios con mayor demanda?
- ¿Cómo varían los precios según el tipo de alojamiento?
- ¿Qué factores más influyen en el precio?
- ¿Cuál es la relación entre precio y valoraciones?
- ¿Cuáles son los alojamientos más competitivos?

---

## 🏗️ Estructura del Proyecto

```
Airbnb Analysis in Madrid/
├── README.md                              # Este archivo
├── codigo_analisis_airbnb_madrid.ipynb   # Notebook con análisis completo
└── presentación_analisis_airbnb_madrid.pdf # Presentación visual de resultados
```

---

## 🔍 Metodología

El análisis sigue el siguiente flujo:

### 1️⃣ **Carga y Exploración de Datos**
- Importación del dataset de Airbnb Madrid
- Verificación de estructura, tipos de datos y calidad
- Identificación de valores faltantes y duplicados

### 2️⃣ **Limpieza y Preparación de Datos**
- Tratamiento de valores nulos
- Conversión de tipos de datos
- Eliminación de outliers cuando sea apropiado
- Normalización de variables categóricas

### 3️⃣ **Análisis Exploratorio (EDA)**
- Estadísticas descriptivas
- Distribuciones de variables clave
- Identificación de patrones y correlaciones
- Análisis por segmentos (barrios, tipos, etc.)

### 4️⃣ **Visualización de Datos**
- Gráficos de distribución (histogramas, boxplots)
- Mapas geográficos con ubicaciones
- Análisis de tendencias temporales
- Correlaciones entre variables

### 5️⃣ **Análisis Estadístico**
- Correlaciones (Pearson, Spearman)
- Tests de hipótesis
- Agrupación de datos (clustering)
- Análisis de segmentación

### 6️⃣ **Generación de Insights**
- Identificación de oportunidades de negocio
- Recomendaciones basadas en datos
- Estrategias de precios

---

## 📊 Datos

### Fuente
Dataset de Airbnb Madrid con información de alojamientos activos

### Variables Principales
| Variable | Descripción | Tipo |
|----------|-------------|------|
| `id` | ID único del alojamiento | Numérico |
| `name` | Nombre del alojamiento | Texto |
| `neighbourhood` | Barrio de Madrid | Categórico |
| `room_type` | Tipo de habitación | Categórico |
| `price` | Precio por noche (€) | Numérico |
| `minimum_nights` | Mínimo de noches | Numérico |
| `number_of_reviews` | Número de reseñas | Numérico |
| `review_scores_rating` | Puntuación promedio | Numérico |
| `availability_365` | Días disponibles/año | Numérico |
| `latitude/longitude` | Coordenadas geográficas | Geográfico |

---

## 📈 Análisis Realizados

### 1. **Análisis de Precios**
- Estadísticas por tipo de alojamiento
- Distribución de precios por barrio
- Variación de precios según características
- Identificación de alojamientos con mejor relación precio-valor

### 2. **Análisis Geográfico**
- Mapas de calor de precios
- Distribución de alojamientos por zona
- Barrios más demandados
- Clusters de ubicaciones similares

### 3. **Análisis de Demanda**
- Relación entre número de reseñas y popularidad
- Disponibilidad vs. ocupación estimada
- Tendencias de demanda por barrio
- Estacionalidad

### 4. **Análisis de Calidad**
- Puntuaciones promedio por categoría
- Relación entre precio y valoraciones
- Factores que mejoran la satisfacción
- Benchmarking competitivo

### 5. **Análisis de Competencia**
- Segmentación de mercado
- Análisis de competidores directos
- Identificación de nichos sin explotar
- Estrategias de posicionamiento

### 6. **Análisis Predictivo**
- Modelos para predicción de precios
- Factores más influyentes
- Escenarios de simulación
- Optimización de estrategias

---

## 🎯 Hallazgos Clave

### 💡 Insights Principales

1. **Distribución de Precios**
   - Rango de precios: €X - €Y por noche
   - Promedio: €Z (mediana: €W)
   - Variación importante según barrio

2. **Barrios Más Demandados**
   - Centro (más caro)
   - Zona turística (más reseñas)
   - Barrios emergentes (mejor relación precio-valor)

3. **Tipos de Alojamiento**
   - Habitaciones completas: mayor precio y demanda
   - Habitaciones compartidas: entrada más económica
   - Apartamentos: volumen más alto

4. **Factores de Éxito**
   - Ubicación es fundamental (X% de varianza explicada)
   - Disponibilidad moderada (50-60 días/año óptimo)
   - Mínimo de noches bajo mejora conversión
   - Puntuaciones altas atraen más reseñas

5. **Oportunidades Detectadas**
   - Segmento de lujo infraexplotado
   - Nichos específicos (mascotas, familias, etc.)
   - Barrios con potencial de crecimiento
   - Falta de alojamientos en ciertos rangos de precio

### 📊 Recomendaciones

**Para Hosts:**
- Optimizar títulos y descripciones (mejor SEO)
- Gestionar precios dinámicamente según estacionalidad
- Mantener valoraciones altas (crítico para conversión)
- Establecer políticas flexibles de cancelación

**Para Inversores:**
- Considerar barrios emergentes con buena accesibilidad
- Enfocarse en apartamentos completos (ROI más alto)
- Diferenciar oferta (pet-friendly, co-working, etc.)
- Planificar para alta estacionalidad

---

## 🛠️ Tecnologías Utilizadas

### Lenguaje & Entorno
- **Python 3.x** - Lenguaje principal
- **Jupyter Notebook** - Entorno interactivo

### Librerías de Análisis
- **Pandas** - Manipulación y análisis de datos
- **NumPy** - Computación numérica
- **Scipy** - Tests estadísticos
- **Scikit-learn** - Machine Learning y preprocesamiento

### Visualización
- **Matplotlib** - Gráficos estáticos
- **Seaborn** - Visualizaciones estadísticas
- **Plotly** - Gráficos interactivos
- **Folium** - Mapas geográficos

### Utilidades
- **GeoPandas** - Análisis geoespacial
- **Statsmodels** - Modelado estadístico

---

## 🚀 Cómo Usar Este Proyecto

### Opción 1: Visualizar en GitHub
1. Accede a [`codigo_analisis_airbnb_madrid.ipynb`](./codigo_analisis_airbnb_madrid.ipynb)
2. GitHub renderiza automáticamente el notebook
3. Explora gráficos y análisis interactivamente

### Opción 2: Ejecutar Localmente

#### Requisitos
```bash
Python 3.7+
pip (gestor de paquetes)
```

#### Instalación
```bash
# Clonar el repositorio
git clone https://github.com/JavierPradal/DataAnalytics-projects.git
cd DataAnalytics-projects/"Airbnb Analysis in Madrid"

# Crear entorno virtual (recomendado)
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate

# Instalar dependencias
pip install -r requirements.txt
```

#### Ejecutar el Análisis
```bash
# Iniciar Jupyter
jupyter notebook codigo_analisis_airbnb_madrid.ipynb

# O usar JupyterLab
jupyter lab codigo_analisis_airbnb_madrid.ipynb
```

### Opción 3: Ver Presentación
- Descarga [`presentación_analisis_airbnb_madrid.pdf`](./presentación_analisis_airbnb_madrid.pdf)
- Visualiza un resumen ejecutivo con gráficos clave y conclusiones
- O accede directamente desde el [enlace de descarga](https://github.com/JavierPradal/DataAnalytics-projects/tree/main/Airbnb%20Analysis%20in%20Madrid)

---

## 📁 Archivos del Proyecto

### `codigo_analisis_airbnb_madrid.ipynb` (2.8 MB)
**Notebook Jupyter completo con:**
- Importación y exploración de datos
- Limpieza y transformación de variables
- Análisis estadístico descriptivo
- Visualizaciones múltiples
- Análisis por segmentos
- Modelado predictivo
- Conclusiones y recomendaciones

**Secciones principales:**
1. Introducción y problema
2. Carga de datos
3. Exploración inicial
4. Limpieza de datos
5. Análisis univariante
6. Análisis bivariante
7. Análisis multivariante
8. Visualizaciones geográficas
9. Análisis de competencia
10. Modelado y predicciones
11. Resumen de insights

### `presentación_analisis_airbnb_madrid.pdf` (20.7 MB)
**Presentación visual profesional con:**
- Portada y objetivos
- Resumen ejecutivo
- Gráficos destacados
- Insights principales
- Recomendaciones estratégicas
- Conclusiones

**Ideal para:**
- Presentaciones a stakeholders
- Reportes ejecutivos
- Compartir hallazgos clave
- Toma de decisiones

---

## 📈 Métricas Clave

| Métrica | Valor | Interpretación |
|---------|-------|-----------------|
| Número de alojamientos | N | Tamaño del mercado |
| Precio promedio | €X | Nivel de precios |
| Puntuación promedio | X/5 | Satisfacción general |
| Ocupación estimada | X% | Demanda relativa |
| Rotación (reseñas/año) | X | Actividad/competitividad |

---

## 💡 Casos de Uso

Este análisis es útil para:

✅ **Hosts actuales** - Optimizar precios y características  
✅ **Propietarios potenciales** - Decidir sobre inversión  
✅ **Inversores inmobiliarios** - Identificar oportunidades  
✅ **Consultores** - Asesorar sobre estrategia de Airbnb  
✅ **Estudiantes** - Aprender técnicas de análisis de datos  
✅ **Investigadores** - Entender mercados de economía colaborativa

---

## 🔄 Actualizaciones y Mejoras Futuras

- [ ] Integración con API de Airbnb para datos en tiempo real
- [ ] Modelo de predicción de demanda más avanzado
- [ ] Análisis de sentimiento en reseñas
- [ ] Dashboard interactivo en Streamlit
- [ ] Comparativa con otros destinos turísticos
- [ ] Análisis de impacto ambiental

---

## 📝 Notas Metodológicas

### Supuestos
- Los datos reflejan situación de mercado real en fecha de captura
- Se asume que las reseñas son representativas de la experiencia general
- Los precios son por noche, excluyendo impuestos y tarifas de servicio

### Limitaciones
- Dataset estático (no captura cambios temporales)
- Algunos campos pueden tener datos faltantes
- Puntuaciones pueden estar sesgadas (principalmente reseñas positivas)
- Correlación no implica causalidad

### Consideraciones Éticas
- Análisis puramente descriptivo sin intención de manipular mercados
- Datos públicos de Airbnb
- Utilizado para investigación y propósitos educativos

---

## 👤 Autor

**Javier Pradal**

- GitHub: [@JavierPradal](https://github.com/JavierPradal)
- Proyecto: DataAnalytics-projects
- Enfoque: Análisis de datos, visualización y business intelligence

---

## 📜 Licencia

Este proyecto se distribuye bajo la Licencia MIT. Ver `LICENSE` para detalles.

---

## 🙏 Agradecimientos

- Dataset de Airbnb Madrid
- Comunidad de Python y análisis de datos
- Librerías open-source: pandas, matplotlib, seaborn, folium, etc.

---

## 📞 Contacto & Colaboración

¿Preguntas, sugerencias o colaboraciones?

- 📧 Abre un issue en GitHub
- 🔗 Contribuye con mejoras (pull requests)
- 💬 Comparte tu feedback

---

## 🎓 Aprender Más

**Recursos relacionados:**
- [Documentación de Pandas](https://pandas.pydata.org/)
- [Seaborn Gallery](https://seaborn.pydata.org/examples.html)
- [Scikit-learn](https://scikit-learn.org/)
- [Folium Maps](https://folium.readthedocs.io/)

---

**Última actualización:** 2024  
**Estado:** ✅ Completo y funcional

---

## 📊 Vista Rápida del Contenido

```
🎯 OBJETIVO
└── Entender mercado Airbnb Madrid

📊 ANÁLISIS
├── Precios y distribución
├── Geografía y ubicación
├── Demanda y disponibilidad
├── Calidad (puntuaciones)
├── Competencia
└── Predictivo

💡 RESULTADOS
├── Insights clave
├── Oportunidades
└── Recomendaciones

🛠️ HERRAMIENTAS
├── Python
├── Pandas & NumPy
├── Matplotlib & Seaborn
└── Scikit-learn

📈 IMPACTO
├── Para hosts
├── Para inversores
├── Para plataforma
└── Para turistas
```

---

**¡Gracias por revisar este análisis! 🎉**
