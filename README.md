# Inteligencia_de_Negocios_UBA_2025

Repositorio privado del trabajo final **“ANÁLISIS PREDICTIVO DE TARIFAS DE VIAJES EN LA PLATAFORMA UBER: APLICACIONES DE MODELOS DE APRENDIZAJE AUTOMÁTICO EN INTELIGENCIA DE NEGOCIOS”**.

Este proyecto corresponde al **remanente octubre 2025** de la asignatura **Inteligencia de Negocios**, Maestría en Economía Aplicada (FCE–UBA).  
Integra técnicas de *Business Intelligence* y *Machine Learning* para el análisis y predicción de tarifas en la plataforma **UBER**, utilizando modelos lineales, ensambles y redes neuronales.

---

## 📂 Estructura del repositorio

Inteligencia_de_Negocios_UBA_2025/
│
├── data/ # Dataset original (uber.csv)
│
├── notebooks/
│ └── tp_final_bi_2025_delgadillo.ipynb # Notebook principal (EDA, modelos, resultados)
│
├── figures/ # Gráficos y visualizaciones generadas
│
├── Informe_Final_Remanente/ # Informe LaTeX y versión PDF final
│
├── README.md # Este archivo de documentación
└── requirements.txt # Dependencias del entorno (opcional)

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
