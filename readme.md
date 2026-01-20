
# Evaluación final módulo 3

**Descripción breve del proyecto**  
Análisis exploratorio de datos de vuelos y programas de fidelidad. Se realiza limpieza (nulos en Salary/College), EDA estadístico, visualizaciones de distribuciones y correlaciones para insights de negocio en el contexto de evaluación bootcamp Adalab Módulo 3.

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

## 🚀 Instrucciones de uso

### 1️⃣ Clonar repositorio
```bash
# Clonar repositorio de GitHub
git clone https://github.com/cristinaragon/bda-modulo-3-evaluacion-final-cristinaragon.git
cd bda-modulo-3-evaluacion-final-cristinaragon
2️⃣ Instalar dependencias
bash
pip install -r requirements.txt
3️⃣ Descargar datasets
Colocar en data/raw/:

Customer Flight Activity.csv [400.500 registros]

Customer Loyalty History.csv [16.700 clientes]

Descripción general
Este proyecto forma parte de la evaluación final del Módulo 3 de Análisis de Datos e Inteligencia Artificial del bootcamp Adalab. Se centra en el análisis exploratorio de dos datasets relacionados con reservas de vuelos (Customer Flight Activity.csv) y programas de fidelidad de clientes (Customer Loyalty History.csv).

El objetivo es aplicar todo lo aprendido: limpieza de datos (manejo de nulos como Salary con 25% missing y College), análisis estadístico descriptivo (medias, varianzas, outliers con IQR), análisis de correlaciones, visualizaciones y preparación para modelado.

🎯 Objetivos
Objetivo principal
Realizar un análisis exploratorio de datos (EDA) completo sobre reservas de vuelos y programas de fidelidad, identificando patrones en variables como salario, provincia, college, y comportamientos de clientes para generar insights de negocio.

Objetivos específicos
Limpieza de datos: Manejar nulos (Salary 25%, College), outliers IQR, tipos de datos

Análisis estadístico: Medidas centrales, dispersión, distribuciones numéricas/categóricas

Visualizaciones EDA: Histogramas, boxplots, frecuencias por provincia, correlaciones

Patrones: Relaciones salario/college/provincia/fidelidad vuelos

Preparación modelado: Validación datos y feature engineering

📊 Dataset
Dataset 1: Reservas de vuelos (Customer Flight Activity.csv)
Característica	Descripción
Filas	400.500 registros
Columnas	~15-20 columnas
Variables clave	Origen, destino, fecha, duración, precio
Problemas	Tipos fecha/hora por ajustar
Dataset 2: Fidelidad clientes (Customer Loyalty History.csv)
Característica	Descripción
Filas	16.700 clientes
Columnas	~10-15 columnas
Variables clave	Salary (25% nulos), College, provincia
Problemas	Salary 25% missing, outliers
Merge: pd.merge(df_flights, df_loyalty, on='loyalty_number', how='inner')

📈 Notas técnicas:

Salary: Imputación groupby provincia/college → media

Outliers: Método IQR en precio/duración

Feature engineering: precio_por_hora = precio/duración

🛠️ Tecnologías
python
# Entorno principal
Python 3.9+
pandas, numpy
matplotlib, seaborn
jupyter notebook
📁 Estructura del proyecto
text
bda-modulo-3-evaluacion-final-cristinaragon/
├── data/
│   ├── Customer Flight Activity.csv
│   └── Customer Loyalty History.csv
├── notebooks/
│   ├── Analisis_Loyalty.ipynb
│   └── 03_visualizaciones.ipynb
└── README.md
______ graficos/
    ├── boxplots/
    ├── histogramas/
    └── correlaciones/
🔄 Metodología
Limpieza: Nulos Salary/College, outliers IQR, tipos datos

EDA estadístico: Descriptivos, correlaciones, distribuciones

Visualizaciones: Boxplots, histogramas, frecuencias provincia

Feature engineering: precio_por_hora, fidelidad_alta

Validación: Calidad datos post-procesado

📈 Resultados
Insights Salary vs fidelidad por provincia

Patrones outliers precio/duración vuelos

Correlaciones variables numéricas clave

⚠️ Retos y mejoras
Retos:

25% nulos Salary → imputación compleja

Merge loyalty_number → pérdida filas inner join

Mejoras:

Modelos predictivos churn fidelidad

Dashboard Streamlit/PowerBI

👩‍💻 Autora
Cristina Aragón
Estudiante Bootcamp Data Analysis
Adalab - Módulo 3/4 (Análisis de Datos e IA)

GitHub

📧 Contacto: cristinaragon77@gmail.com
📅 Entrega: Enero 2026 - Evaluación Final Módulo 3

Proyecto desarrollado durante bootcamp Adalab para demostrar competencias en limpieza, EDA y visualización de datos.
