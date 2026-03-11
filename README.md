<h1 align = "center">  
📊 Análisis de Evasión de Clientes - Telecom X</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Estado-Terminado-brightgreen" />
</p>

Este proyecto tiene como objetivo analizar los datos de clientes de 
Telecom X para identificar los factores asociados a la evasión 
(churn), es decir, la cancelación del servicio por parte de los 
usuarios. A través de un análisis exploratorio de datos, se busca 
generar insights accionables que ayuden a reducir la tasa de 
cancelación y mejorar la retención de clientes.

## 🎯 Objetivos del Análisis
- Explorar y limpiar el conjunto de datos de clientes.
- Identificar variables categóricas y numéricas asociadas a la evasión.
- Analizar la distribución de la evasión según distintos perfiles de cliente.
- Visualizar patrones relevantes mediante gráficos comparativos.
- Proponer conclusiones y recomendaciones estratégicas basadas en los resultados.

## 🛠️ Tecnologías usadas
- Python 3 como lenguaje de programación
- Google Colab como entorno de desarrollo
- Pandas para manipulación y análisis de datos
- NumPy para cálculos numéricos
- Matplotlib para visualización de datos
- Seaborn para visualizaciones estadísticas avanzadas

## 📂 Estructura del proyecto
```
Proyecto
├── TelecomX_Data.json
├── ChallengePart1.ipynb
└── README.md
```

## 🔎 Metodología
1. Extracción y carga de datos
    - Lectura del archivo JSON con pandas.
    - Visualización inicial del dataset.

2. Transformación y limpieza
    - Normalización de columnas con datos en formato diccionario.
    - Eliminación de duplicados y valores vacíos.
    - Conversión de variables binarias a formato numérico (0/1).
    - Estandarización de valores como "No internet service" y 
      "No phone service".
    - Creación de columna adicional: Cuentas_Diarias.

3. Análisis exploratorio
    - Análisis descriptivo general del dataset.
    - Distribución de la variable objetivo (Churn).
    - Tasa de evasión por variables categóricas 
      (género, tipo de contrato, método de pago, 
      servicio de internet).
    - Distribución de variables numéricas 
      (tenure, Charges.Monthly, Charges.Total) 
      según evasión.

4. Visualización
    - Gráfico de torta para distribución de Churn.
    - Gráficos de barras para variables categóricas.
    - Gráficos de densidad (KDE) para variables numéricas.

## 📌 Principales Hallazgos
- El 26.2% de los clientes canceló el servicio.
- Los contratos mes a mes presentan la mayor tasa de evasión (42.02%).
- Los usuarios de Fibra óptica cancelan más que otros (41.21%).
- Los clientes que pagan con cheque electrónico tienen la tasa 
  más alta de evasión (44.47%).
- Los clientes nuevos son los más vulnerables, con la mayoría 
  de cancelaciones ocurriendo en los primeros meses.
- Los cargos mensuales altos están asociados a mayor evasión.
- El género no es un factor determinante en la cancelación.

## 🏁 Conclusión
El análisis reveló que los factores más críticos asociados a la 
evasión son el tipo de contrato, el servicio de internet contratado 
y el método de pago. Los clientes nuevos con contratos mensuales, 
servicio de fibra óptica y pago manual representan el perfil de 
mayor riesgo. Estas variables pueden ser clave para desarrollar 
estrategias de retención más efectivas.

## ▶ Cómo Ejecutar el Proyecto
- Clonar el repositorio:
```bash
git clone https://github.com/tu-usuario/telecomx-churn-analysis.git
```
- Instalar dependencias:
```bash
pip install pandas numpy matplotlib seaborn
```
- Ejecutar el notebook:
Abrir el archivo `ChallengePart1.ipynb` en Jupyter Notebook 
o Google Colab.

## 📌 Posibles Mejoras Futuras
- Implementar un modelo predictivo de evasión (Machine Learning).
- Incorporar visualizaciones interactivas con Plotly.
- Ampliar el análisis con segmentación de clientes.
- Análisis de rentabilidad por tipo de servicio contratado.
