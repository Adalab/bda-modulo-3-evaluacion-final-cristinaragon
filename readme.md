# Evluación final módulo 3
## 🚀 Instrucciones de uso

### 1️⃣ Clonar repositorio
```bash
#Clonar repositorio de GitHub
git clone bda-modulo-3-evaluacion-final-cristinaragon en la carpeta del proyecto que deseas trabajar

**Descripción breve del proyecto** Análisis exploratorio de datos de vuelos y programas de fidelidad. Se realiza limpieza (nulos en Salary/College), EDA estadístico, visualizaciones de distribuciones y correlaciones para insights de negocio en el contexto de evaluación bootcamp Adalab Módulo 3.

### Instalar dependencias

```bash
pip install -r requirements.txt

## Descargar datasets
Descargar los datasets desde los siguientes enlaces y colocarlos en la carpeta `data/` del proyecto:
- [Customer Flight Activity.csv](enlace_al_dataset_1)
- [Customer Loyalty History.csv](enlace_al_dataset_2)

## 📋 Índice

- [Descripción general]
- [Objetivos]
- [Dataset]
- [Tecnologías]
- [Estructura del proyecto]
- [Metodología]
- [Instrucciones de uso]
- [Resultados]
- [Retos y mejoras]
- [Autora]

## Descripción general

Este proyecto forma parte de la **evaluación final del Módulo 3 de Análisis de Datos e Inteligencia Artificial** del bootcamp Adalab. Se centra en el análisis exploratorio de dos datasets relacionados con **reservas de vuelos** (`Custormer Flight Activity.csv`) y **programas de fidelidad de clientes** (`Customer Loyalty History.csv`).

El objetivo es aplicar todo lo aprendido: **limpieza de datos** (manejo de nulos como Salary con 25% missing y College), **análisis estadístico descriptivo** (medias, varianzas, outliers con IQR), **análisis de correlaciones**, **visualizaciones** (distribuciones categóricas/numéricas) y **preparación para modelado**.

Los insights generados ayudarán a entender patrones en vuelos, salarios, provincias y comportamientos de clientes leales, preparando la base para decisiones de negocio y defensa en entrevista técnica.


## 🎯 Objetivos

### Objetivo principal
Realizar un análisis exploratorio de datos (EDA) completo sobre reservas de vuelos y programas de fidelidad, identificando patrones en variables como salario, provincia, college, y comportamientos de clientes para generar insights de negocio que sirvan de base para decisiones estratégicas y modelado predictivo.

### Objetivos específicos
- **Limpieza de datos**: Manejar nulos (Salary 25%, College), detectar y tratar outliers con IQR, ajustar tipos de datos
- **Análisis estadístico descriptivo**: Calcular medidas centrales (media, mediana), dispersión (varianza, desviación estándar) y distribuciones de variables numéricas/categóricas
- **Análisis exploratorio visual (EDA)**: Crear visualizaciones de distribuciones (histogramas, boxplots), frecuencias por provincia y correlaciones entre variables
- **Identificación de patrones**: Analizar relaciones entre salario, college, provincia y comportamientos de fidelidad en vuelos
- **Preparación para modelado**: Validar calidad de datos y generar features para futuros modelos predictivos


## 📊 Dataset

### Dataset 1: Reservas de vuelos (`Customer Flight Activity.csv`)
| Característica | Descripción |
|----------------|-------------|
| **Filas** | [400.500 registros de vuelos] |
| **Columnas** | [~15-20 columnas] |
| **Variables clave** | Origen, destino, fecha, duración, precio, provincia |
| **Problemas identificados** | [Nulos mínimos, tipos fecha/hora por ajustar] |

### Dataset 2: Fidelidad clientes (`Customer Loyalty History.csv`) 
| Característica | Descripción |
|----------------|-------------|
| **Filas** | [16.700 clientes] |
| **Columnas** | [~10-15 columnas] |
| **Variables clave** | **Salary** (25% nulos), **College** (NaN tras imputación), provincia, puntuación fidelidad |
| **Problemas identificados** | **Salary: 25% missing** (imputado por grupos), outliers, tipos object |

## 🛠️ Tecnologías

```python
# Entorno principal
Python 3.9+
pandas, numpy
matplotlib, seaborn, plotly
jupyter notebook
