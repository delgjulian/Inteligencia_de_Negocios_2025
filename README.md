# Inteligencia_de_Negocios_UBA_2025

Repositorio del proyecto “Análisis predictivo de tarifas de viajes en la plataforma Uber: aplicaciones de modelos de aprendizaje automático en inteligencia de negocios”.

Este trabajo desarrolla un enfoque empírico para el análisis y predicción de tarifas de viajes en la plataforma Uber, integrando técnicas de Business Intelligence y Machine Learning. El proyecto combina exploración de datos, modelado econométrico y algoritmos de aprendizaje automático para evaluar el desempeño predictivo de distintos enfoques.

El estudio fue desarrollado en el marco de la Maestría en Economía Aplicada (FCE – Universidad de Buenos Aires) y se presenta aquí como un proyecto académico reproducible, con datos, código y documentación completa.

---

## 📂 Estructura del repositorio

Inteligencia_de_Negocios_2025/
│
├── data/                         # Dataset original (uber.csv)
│
├── notebooks/
│   └── uber_fare_prediction.ipynb # Notebook principal (EDA, modelos y resultados)
│
├── figures/                      # Gráficos y visualizaciones generadas
│
├── report/                       # Informe final (LaTeX y PDF)
│
├── README.md                     # Documentación del proyecto
└── requirements.txt              # Dependencias del entorno (opcional)

---

## 🧾 Descripción del trabajo

El objetivo es **modelar y predecir el valor de las tarifas UBER** a partir de variables geoespaciales y de distancia, empleando las siguientes etapas:

1. **Exploración y limpieza de datos (EDA)**
   - Lectura del dataset `uber.csv`
   - Generación de variable de distancia mediante la fórmula de *Haversine*
   - Correlaciones de Pearson y Spearman  
   - Detección y eliminación de *outliers*

2. **Modelado tradicional**
   - Regresión Lineal (MCO)
   - LASSO (regularización con selección de variables)

3. **Modelos de Aprendizaje Automático**
   - Random Forest  
   - Gradient Boosting  
   - Redes Neuronales (Keras)

4. **Evaluación de performance**
   - Métricas: **RMSE** y **MAE**
   - Comparación y conclusiones de cada modelo

---

## ⚙️ Reproducibilidad

### 🔹 Requisitos básicos

Ejecutar en **Google Colab** o entorno local con Python 3.10+  
Dependencias principales:

```bash
pip install numpy pandas scikit-learn tensorflow matplotlib seaborn

