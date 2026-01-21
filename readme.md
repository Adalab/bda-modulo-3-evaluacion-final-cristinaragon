# 📊 Evaluación final – Módulo 3

## Descripción breve del proyecto
Análisis exploratorio de datos (EDA) de vuelos y programas de fidelidad.  
Se realiza limpieza de datos (nulos en `Salary` y `College`), análisis estadístico, visualizaciones de distribuciones y correlaciones para la obtención de insights de negocio, en el contexto de la **evaluación del Módulo 3 del bootcamp Adalab**.

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

## 📌 Descripción general
Este proyecto forma parte de la **evaluación final del Módulo 3 de Análisis de Datos e Inteligencia Artificial** del bootcamp **Adalab**.

Se centra en el análisis exploratorio de dos datasets relacionados con:
- **Reservas de vuelos** (`Customer Flight Activity.csv`)
- **Programas de fidelidad de clientes** (`Customer Loyalty History.csv`)

---

## 🎯 Objetivos

### Objetivo principal
Realizar un análisis exploratorio de datos completo sobre reservas de vuelos y programas de fidelidad, identificando patrones en variables como salario, provincia, nivel educativo y comportamiento del cliente, para generar **insights de negocio**.

---

## 📊 Dataset

### Dataset 1: Reservas de vuelos
**Customer Flight Activity.csv**

| Característica | Descripción |
|--------------|------------|
| Filas | ~400.500 registros |
| Columnas | 15–20 |

---

### Dataset 2: Fidelidad de clientes
**Customer Loyalty History.csv**

| Característica | Descripción |
|--------------|------------|
| Filas | ~16.700 clientes |
| Columnas | 10–15 |

---

### Merge de datasets
python
pd.merge(df_flights, df_loyalty, on='loyalty_number', how='inner')
## 🛠️ Tecnologías
- **Python 3.9+**
- **pandas**
- **numpy**
- **matplotlib**
- **seaborn**
- **Jupyter Notebook**

---
## 📁 Estructura del proyecto
bda-modulo-3-evaluacion-final-cristinaragon/
├── data/
│   ├── raw/
│   │   ├── Customer Flight Activity.csv
│   │   └── Customer Loyalty History.csv
│   └── processed/
├── notebooks/
│   ├── Análisis_Loyalty.ipynb
├── graficos/
│   ├── boxplots/
│   ├── histogramas/
│   └── correlaciones/
├── requirements.txt
└── README.md
---

## 🔄 Metodología
- **Limpieza de datos**
  - Imputación de valores nulos en `Salary` mediante `groupby` por provincia y nivel educativo
- **EDA**
  - Análisis de distribuciones
  - Detección de outliers mediante el método IQR
- **Visualización**
  - Gráficos comparativos para analizar el comportamiento de los clientes

---

## 👩‍💻 Autora
**Cristina Aragón**  
Estudiante del Bootcamp de Data Analysis – Adalab  

📧 cristinaragon77@gmail.com  
📅 Enero 2026


