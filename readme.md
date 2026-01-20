# Evaluación final módulo 3

**Descripción breve del proyecto** Análisis exploratorio de datos de vuelos y programas de fidelidad. Se realiza limpieza (nulos en Salary/College), EDA estadístico, visualizaciones de distribuciones y correlaciones para insights de negocio en el contexto de evaluación bootcamp Adalab Módulo 3.

---

## 📋 Índice
- [Descripción general](#descripción-general)
- [Objetivos](#objetivos)
- [Dataset](#dataset)
- [Tecnologías](#tecnologías)
- [Estructura del proyecto](#estructura-del-proyecto)
- [Metodología](#metodología)
- [Instrucciones de uso](#instrucciones-de-uso)
- [Resultados](#resultados)
- [Retos y mejoras](#retos-y-mejoras)
- [Autora](#autora)

---

## ## Descripción general
Este proyecto forma parte de la **evaluación final del Módulo 3 de Análisis de Datos e Inteligencia Artificial** del bootcamp Adalab. Se centra en el análisis exploratorio de dos datasets relacionados con **reservas de vuelos** (`Customer Flight Activity.csv`) y **programas de fidelidad de clientes** (`Customer Loyalty History.csv`).

El objetivo es aplicar todo lo aprendido: **limpieza de datos** (manejo de nulos como Salary con 25% missing y College), **análisis estadístico descriptivo** (medias, varianzas, outliers con IQR), **análisis de correlaciones**, **visualizaciones** y **preparación para modelado**.

---

## ## 🎯 Objetivos

### ### Objetivo principal
Realizar un análisis exploratorio de datos (EDA) completo sobre reservas de vuelos y programas de fidelidad, identificando patrones en variables como salario, provincia, college, y comportamientos de clientes para generar insights de negocio.

### ### Objetivos específicos
- **Limpieza de datos**: Manejar nulos (Salary 25%, College), outliers IQR, tipos de datos.
- **Análisis estadístico**: Medidas centrales, dispersión, distribuciones numéricas/categóricas.
- **Visualizaciones EDA**: Histogramas, boxplots, frecuencias por provincia, correlaciones.
- **Patrones**: Relaciones salario/college/provincia/fidelidad vuelos.
- **Preparación modelado**: Validación datos y feature engineering.

---

## ## 📊 Dataset

### ### Dataset 1: Reservas de vuelos (`Customer Flight Activity.csv`)
| Característica | Descripción |
| :--- | :--- |
| **Filas** | 400.500 registros |
| **Columnas** | ~15-20 columnas |
| **Variables clave** | Origen, destino, fecha, duración, precio |
| **Problemas** | Tipos fecha/hora por ajustar |

### ### Dataset 2: Fidelidad clientes (`Customer Loyalty History.csv`)
| Característica | Descripción |
| :--- | :--- |
| **Filas** | 16.700 clientes |
| **Columnas** | ~10-15 columnas |
| **Variables clave** | **Salary** (25% nulos), College, provincia |
| **Problemas** | **Salary 25% missing**, outliers |

**Merge**: `pd.merge(df_flights, df_loyalty, on='loyalty_number', how='inner')`

---

## ## 🛠️ Tecnologías
```python
# Entorno principal
Python 3.9+
pandas, numpy
matplotlib, seaborn
jupyter notebook

## ## 📁 Estructura del proyecto
Plaintext

bda-modulo-3-evaluacion-final-cristinaragon/
├── data/raw/
│   ├── Customer Flight Activity.csv
│   └── Customer Loyalty History.csv
├── data/processed/
├── notebooks/
│   ├── 01_limpieza.ipynb
│   ├── 02_eda.ipynb
│   └── 03_visualizaciones.ipynb
├── graficos/
│   ├── boxplots/
│   ├── histogramas/
│   └── correlaciones/
├── requirements.txt
└── README.md
## 🚀 Instrucciones de uso
### 1. Clonar repositorio
Bash

git clone [https://github.com/cristinaragon/bda-modulo-3-evaluacion-final-cristinaragon.git]

### 2. Instalar dependencias
Bash

pip install -r requirements.txt

### 3. Ejecutar Notebooks
Asegúrate de tener los archivos .csv en la carpeta data/raw/.

Abre VS Code y ejecuta los archivos en la carpeta notebooks/ en el orden indicado: 01_limpieza -> 02_eda -> 03_visualizaciones.

## 🔄 Metodología
Limpieza: Imputación de nulos en Salary mediante groupby por provincia y estudios.

EDA: Análisis de tendencias y detección de valores atípicos (outliers).

Visualización: Creación de gráficos comparativos para entender el comportamiento de los clientes.

## 👩‍💻 Autora
Cristina Aragón Estudiante Bootcamp Data Analysis - Adalab

📧 cristinaragon77@gmail.com

📅 Enero 2026