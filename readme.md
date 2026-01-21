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
```python
pd.merge(df_flights, df_loyalty, on='loyalty_number', how='inner')
🛠️ Tecnologías
Python 3.9+

pandas

numpy

matplotlib

seaborn

Jupyter Notebook

📁 Estructura del proyecto
plaintext
Copiar código
bda-modulo-3-evaluacion-final-cristinaragon/
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
├── graficos/
├── requirements.txt
└── README.md
👩‍💻 Autora
Cristina Aragón
Estudiante Bootcamp Data Analysis – Adalab
📅 Enero 2026
