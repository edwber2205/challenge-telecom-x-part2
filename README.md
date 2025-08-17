# 🤖 Challenge Telecom X Parte 2: Predicción de Evasión de Clientes

## 📌 Descripción del Proyecto
En esta segunda parte del desafío, el objetivo es **predecir qué clientes tienen mayor probabilidad de abandonar la empresa Telecom X**.  
A partir del dataset tratado en la Parte 1, se implementarán modelos de Machine Learning para anticipar la evasión y proporcionar información estratégica para la retención de clientes.

---

## 🎯 Objetivos del Proyecto

- **General:** 
- Desarrollar y evaluar modelos predictivos que permitan identificar clientes con alto riesgo de evasión.

- **Específicos:**
  - Preparar y transformar los datos para modelado predictivo.
  - Realizar análisis de correlación y selección de variables.
  - Entrenar y evaluar modelos utilizando métricas de clasificación.
  - Analizar la importancia de las variables en el modelo.
  - Predecir el **churn** (cancelación) de clientes de Telecom X.
  - Generar una estrategia de prevención basada en los datos analizados.
  - Elaborar conclusiones y recomendaciones estratégicas.

---

## 📊 Descripción de los datos
La base de datos utilizada proviene de la etapa anterior del presente proyecto, donde se realizó exploración y limpieza de los datos, los cuales pueden obtenerse en el siguiente enlace:

<a href="https://github.com/ignaciomajo/proyecto_TelecomX/tree/main/src">Contenedor Base de Datos</a>

📄 Se tomaron los archivos: 

* <a href="https://raw.githubusercontent.com/ignaciomajo/proyecto_TelecomX/refs/heads/main/src/preprocessed_TelecomX_data.json">preprocessed_TelecomX_data.json</a>
* <a href="https://raw.githubusercontent.com/ignaciomajo/proyecto_TelecomX/refs/heads/main/src/clientes_altovalor_abandonan.json">clientes_altovalor_abandonan.json</a>

Ambos archivos se integraron en un único dataset de **7152 observaciones**. El archivo **clientes_altovalor_abandonan.json** contiene los clientes identificados como outliers en la etapa anterior, que, aunque fueron apartados para un análisis aislado, se incluyeron en este proyecto para representar con mayor fidelidad el patrón general de comportamiento del cliente.

---

## 🧪 Proceso de Preparación de datos

1. **Clasificación de variables:**
- Variables categóricas: Género, tipo de contrato, servicio de internet, etc.
- Variables numéricas: Tenure, MonthlyCharges, TotalCharges, etc.

2. **Tratamiento de datos:**
- Conversión de TotalCharges a formato numérico.
- Eliminación de columnas irrelevantes para el modelo.
- Codificación de variables categóricas con One-Hot Encoding.

3. **Normalización:**
- Se aplicó StandardScaler para escalar las variables numéricas.

4. **División del dataset:**
- Entrenamiento: 80%
- Prueba: 20%

5. **Modelos utilizados:**
- Logistic Regression
- Random Forest
- XGBoost
- KNN
- SVM

6. **Evaluación de modelos:**
- Accuracy, Precision, Recall, F1-score
- Curva ROC y matriz de confusión

---

## 📊 Visualizaciones y Resultados

- Gráficos de correlación para selección de variables.
- Matriz de confusión y curvas ROC para comparar desempeño de modelos.
- Análisis de importancia de variables con Random Forest y XGBoost.
- Insights claros sobre qué perfiles presentan mayor riesgo de churn.

---

## 🛠 Herramientas y Tecnologías
- **Lenguaje:** Python  
- **Librerías:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost 
- **Control de Versiones:** Git y GitHub
- **Entorno de ejecución:** Google Colab. 

---

## 🚀 Flujo de Trabajo Propuesto
1. **Carga de datos tratados** (desde el proyecto Parte 1).
2. **Preparación adicional** para modelos (normalización, codificación, etc.).
3. **Análisis exploratorio y correlación** de variables.
4. **Entrenamiento de modelos predictivos**.
5. **Evaluación de modelos** con métricas como Accuracy, Recall, Precision y F1-score.
6. **Interpretación y conclusiones estratégicas**.

---

## 📅 Gestión del Proyecto
Se utilizará **Trello** como herramienta de colaboración y gestión de tareas, siguiendo las fases y pasos definidos en el tablero del desafío.

---

## 🚀 Instrucciones de Ejecución

1. Abre el cuaderno proyecto_telecomX_ML.ipynb en Google Colab.
2. Asegúrate de tener el archivo dados_tratados.csv en el mismo entorno de ejecución.
3. Instala las bibliotecas necesarias (si no están disponibles):

---

## 📄 Entregables Finales
- Notebook con análisis, modelado y conclusiones.
- Dataset listo para uso predictivo.
- Visualizaciones y métricas clave.
- Informe final con recomendaciones para reducir la evasión.

---

## 👏 Créditos y Reconocimientos
Este proyecto está basado en los datos tratados en el **Challenge Telecom X Parte 1**.  
Fue desarrollado con base en el cuaderno compartido por **Ignacio Majo** compañero de grupo de estudio, a quien agradezco por el aporte en la estructura y el enfoque del análisis.  
Se ha adaptado y enriquecido con explicaciones, visualizaciones y mejoras propias como parte del aprendizaje individual en ciencia de datos.

---

## 📬 Contacto
👤 Autor: Edwin Berrío - Analista de datos junior
Repositorio: github.com/edwber2205
Proyecto: Challenge Telecom X - Parte 2