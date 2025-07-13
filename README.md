# 🧠 Diagnóstico de Cáncer Colorrectal con Deep Learning

Este proyecto consiste en una aplicación de diagnóstico automático de cáncer colorrectal mediante el análisis de imágenes de tejido, usando modelos de Deep Learning como CNN simple, ResNet50 y DenseNet121.

---

## 📌 Objetivo

Desarrollar una herramienta interactiva que permita:

- Clasificar imágenes de tejido colorectal en 14 clases.
- Evaluar modelos entrenados y visualizar resultados.
- Generar reportes PDF con métricas, gráficos y análisis estadísticos.
- Mostrar resultados de predicción a través de una interfaz web desarrollada con Streamlit.

---

## 🗂️ Estructura del Proyecto

Diagnostico Cancer Colorrectal DeepLearning/
├── Notebook/

│ └── Diagnostico Cancer Colorrectal.ipynb ← Notebook principal en Google Colab

├── Modelos/

│ └── README_modelos.md ← Instrucciones con enlace de descarga de modelos (.h5, .pkl)

├── Evaluacion de Modelos/

│ ├── resumen_metricas.csv ← Métricas generales por modelo

│ ├── mcnemar_resultados.csv ← Resultados estadísticos McNemar

│ ├── predicciones_modelos.csv ← Predicciones completas

│ ├── classification_report_.csv ← Reportes detallados por clase
├── Graficas/

│ ├── confusion_matrix_.png ← Matrices de confusión

│ ├── roc_curve_.png ← Curvas AUC-ROC

│ └── precision_recall_.png ← Curvas Precision-Recall

├── dataset_info/

│ ├── README_dataset.md ← Información general del dataset
│ ├── dataset_description.txt ← Descripción del contenido
│ ├── dataset_structure.txt ← Estructura y clases
│ ├── dataset_license.txt ← Licencia
│ └── dataset_source.txt ← Fuente del dataset
├── README.md ← Este archivo

---

## 🧪 Dataset

- **Nombre:** Colorectal Cancer Histology Dataset (CRCCD-V1)
- **Fuente:** Kaggle  
- **Link oficial:** [https://www.kaggle.com/datasets/abpdash/crccd-v1](https://www.kaggle.com/datasets/abpdash/crccd-v1)
- **Número de clases:** 14  
- **Clases:**
  - `ASCENDINGCOLON_ADENOCARCINOMA`
  - `CASIGMOID_COLON`
  - `CECUM`
  - `COLONADENOCARCINOMA`
  - `ESOPHAGITIS`
  - `HEMORRHOID_suspected_CA_colon`
  - `ILEOCECAL_GROWTH`
  - `POLYPS`
  - `PYLORUS`
  - `RECTADENOCARCINOMA`
  - `RECTGROWTH`
  - `SQUAMUS_CELL_ANAL_CARCINOMA`
  - `ULCERATIVE_COLITIS`
  - `Z_LINE`

---

## 🖥️ Tecnologías Usadas

- Python 3.10+
- TensorFlow 2.13+
- scikit-learn
- Streamlit 1.25+
- FPDF
- Matplotlib / Seaborn
- Ngrok (para exponer la app desde Colab)

---

## 📉 Modelos Aplicados

- ✅ CNN Simple (construida desde cero)
- ✅ ResNet50 (Transfer Learning)
- ✅ DenseNet121 (Transfer Learning)

---

## 📈 Métricas Evaluadas

- Accuracy
- Precision / Recall / F1-Score
- Matthews Correlation Coefficient (MCC)
- Matrices de Confusión
- Curvas ROC/AUC
- Curvas Precision/Recall
- Prueba estadística de McNemar

---

## 📄 Reporte PDF Generado

Desde la app de Streamlit se puede descargar un informe PDF que contiene:

- Tabla resumen de métricas
- Gráficos de matrices de confusión
- Curvas ROC y Precision/Recall
- Resultados de la prueba de McNemar
- Interpretaciones automáticas de los modelos

---

## 🚀 Cómo Ejecutar la App

### En Google Colab
Ejecutar el archivo Diagnostico Cancer Colorrectal.ipynb que está dentro de la carpeta Notebook desde Google Colab

## 🔗 Enlace a Modelos
Los modelos .h5 y archivos grandes no están en el repositorio debido a los límites de GitHub. Puedes descargarlos desde Google Drive:

🔗 Modelos entrenados y archivos de evaluación

(El enlace exacto está en el archivo Modelos/README_modelos.md)

## 🤝 Contribuciones
Si deseas colaborar, mejorar el código, agregar pruebas u optimizar el diseño de la app, ¡eres bienvenido! Haz un fork del repositorio y crea un pull request.

## 📜 Licencia
Este proyecto es de uso académico y educativo sin fines de lucro.
El dataset pertenece a sus autores originales y está alojado en Kaggle.
