# Análisis Exploratorio: Propinas en Restaurantes (Dataset Tips)

Notebook de análisis exploratorio de datos (EDA) en Python, desarrollado como parte de un curso de análisis de datos. Explora los factores que influyen en el monto y porcentaje de propinas otorgadas en un restaurante, usando el dataset clásico `tips` de Seaborn.

## 🎯 Objetivo

Identificar patrones de comportamiento en las propinas según variables demográficas y contextuales (sexo, día, horario, hábito de fumar, tamaño del grupo), comparando tanto el monto absoluto de propina como el porcentaje que representa sobre la cuenta total.

## 📊 Contenido del análisis

El notebook desarrolla 12 visualizaciones (gráficos de barras y dispersión) organizadas en dos bloques:

**Propina en valor absoluto, según:**
- Sexo · Día de la semana · Horario (almuerzo/cena) · Fumador vs. no fumador
- Combinaciones: día×sexo, horario×sexo, fumador×sexo
- Tamaño del grupo (relación y magnitud de propina)

**Propina en porcentaje sobre la cuenta** (`tip_percentage`), según:
- Sexo · Día de la semana · Horario · Fumador vs. no fumador

### Hallazgos principales
- En **monto absoluto**, los hombres tienden a dar propinas más altas que las mujeres, especialmente los domingos y durante la cena
- Al analizar en **términos porcentuales**, el patrón se invierte: las mujeres dan un mayor porcentaje de propina respecto a la cuenta
- El tamaño del grupo se relaciona positivamente con el monto de propina
- Ser fumador o no tiene un efecto mínimo sobre el monto, aunque un efecto ligero sobre el porcentaje

## 🛠️ Herramientas utilizadas

- **Python** — pandas, numpy, matplotlib, seaborn
- Dataset: `tips` (incluido en la librería Seaborn)

## 📂 Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `Análisis_propinas.ipynb` | Notebook completo con las 12 visualizaciones y su interpretación |

## ▶️ Cómo ejecutarlo

1. Descarga el notebook
2. Ábrelo con **Jupyter Notebook/Lab** o en **Google Colab**
3. Instala las dependencias si es necesario:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
4. Ejecuta las celdas en orden — el dataset se carga directamente con `sns.load_dataset("tips")`, sin necesidad de archivos externos

---
*Proyecto desarrollado como práctica de análisis de datos con Python.*
