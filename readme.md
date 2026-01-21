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

El objetivo es aplicar los conocimientos adquiridos en:
- Limpieza de datos
- Análisis estadístico descriptivo
- Detección de outliers
- Análisis de correlaciones
- Visualización de datos
- Preparación del dataset para futuros modelos

---

## 🎯 Objetivos

### Objetivo principal
Realizar un análisis exploratorio de datos completo sobre reservas de vuelos y programas de fidelidad, identificando patrones en variables como salario, provincia, nivel educativo y comportamiento del cliente, para generar **insights de negocio**.

### Objetivos específicos
- Limpieza de datos:
  - Tratamiento de valores nulos (`Salary` con ~25% de missing, `College`)
  - Corrección de tipos de datos
  - Gestión de outliers mediante IQR
- Análisis estadístico:
  - Medidas de tendencia central y dispersión
  - Distribuciones de variables numéricas y categóricas
- Visualizaciones:
  - Histogramas
  - Boxplots
  - Frecuencias por provincia
  - Matrices de correlación
- Identificación de patrones:
  - Relación entre salario, nivel educativo, provincia y fidelidad
- Preparación de datos para modelado:
  - Validación de calidad
  - Feature engineering básico

---

## 📊 Dataset

### Dataset 1: Reservas de vuelos  
**`Customer Flight Activity.csv`**

| Característica | Descripción |
|--------------|------------|
| Filas | ~400.500 registros |
| Columnas | 15–20 |
| Variables clave | Origen, destino, fecha, duración, precio |
| Problemas detectados | Tipos de datos en fechas y horas |

---

### Dataset 2: Fidelidad de clientes  
**`Customer Loyalty History.csv`**

| Característica | Descripción |
|--------------|------------|
| Filas | ~16.700 clientes |
| Columnas | 10–15 |
| Variables clave | `Salary`, `College`, provincia |
| Problemas detectados | `Salary` con ~25% de valores nulos, outliers |

**Merge de datasets:**
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
│   │   ├── Customer Flight Activity.csv
│   │   └── Customer Loyalty History.csv
│   └── processed/
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
🔄 Metodología
Limpieza de datos

Imputación de valores nulos en Salary mediante groupby por provincia y nivel educativo

EDA

Análisis de distribuciones

Identificación de outliers mediante método IQR

Visualización

Gráficos comparativos para analizar el comportamiento de los clientes

🚀 Instrucciones de uso
1️⃣ Clonar el repositorio
bash
Copiar código
git clone https://github.com/cristinaragon/bda-modulo-3-evaluacion-final-cristinaragon.git
2️⃣ Instalar dependencias
bash
Copiar código
pip install -r requirements.txt
3️⃣ Ejecutar los notebooks
Asegúrate de que los archivos .csv estén en data/raw/.

Ejecuta los notebooks en este orden:

01_limpieza.ipynb

02_eda.ipynb

03_visualizaciones.ipynb

📈 Resultados
Identificación de patrones de comportamiento según salario y nivel educativo

Diferencias significativas entre provincias

Detección de outliers relevantes para el negocio

Dataset limpio y preparado para futuros modelos predictivos

🚧 Retos y mejoras
Explorar técnicas de imputación más avanzadas

Incluir análisis temporal de vuelos

Aplicar modelos de clustering o segmentación de clientes

Automatizar el pipeline de limpieza y EDA

👩‍💻 Autora
Cristina Aragón
Estudiante del Bootcamp de Data Analysis – Adalab

📧 cristinaragon77@gmail.com
📅 Enero 2026
