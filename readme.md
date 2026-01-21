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

## 📁 Estructura del proyecto

```text
bda-modulo-3-evaluacion-final-cristinaragon/
├── data/
│   ├── Customer Flight Activity.csv
│   ├── Customer Loyalty History.csv
│   ├── customer_flight_activity_clean.csv
│   ├── customer_loyalty_history_clean.csv
│   ├── df_merged_clean.csv
│   ├── frecuencias_categoricas.csv
│   └── outliers_todas_columnas.csv
├── notebooks/
│   └── Análisis_Loyalty.ipynb
├── graficos/
│   ├── pregunta1_vuelos_mes.png
│   ├── pregunta2_simple.png
│   ├── pregunta3_provincia.png
│   ├── pregunta4_salario_visual.png
│   ├── pregunta5_tarjetas.png
│   └── pregunta6_civil_genero.png
└── README.md
---
## 🔄 Metodología
- **Exploración y limpieza de datos**
  - Imputación de valores nulos en `Salary` mediante `groupby` por nivel educativo
- **EDA**
  - Análisis de distribuciones
  - Detección de outliers mediante el método IQR
- **Visualización**
  - Gráficos comparativos para analizar el comportamiento de los clientes
- **Análisis estadístico**
  - Pruebas de hipótesis para evaluar diferencias en reservas de vuelos por nivel educativo
- **Evaluación de Diferencias por Nivel Educativo**
Se analizó el impacto del nivel de estudios en el comportamiento de reserva

---

## 👩‍💻 Autora
**Cristina Aragón**  
Estudiante del Bootcamp de Data Analysis – Adalab  

📧 cristinaragon77@gmail.com  
📅 Enero 2026


