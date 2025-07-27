# Challenge3_telecomX_Parte2
 Predicción de Cancelación (Churn)
# Análisis y Modelado de Cancelación de Clientes (Churn)

## Descripción

Este proyecto tiene como objetivo identificar los factores que influyen en la cancelación de clientes (churn) y construir modelos predictivos para anticipar cuándo un cliente puede cancelar su servicio. Se utilizan técnicas de preprocesamiento, balanceo de clases, y distintos modelos de clasificación para evaluar el desempeño.

---

## Dataset

- Archivo: `datos_tratados.csv`
- Variables: incluye características del cliente como duración del contrato, cargos mensuales y totales, tipo de contrato, etc.
- Variable objetivo: `Churn` (1 = cliente canceló, 0 = cliente activo)

---

## Pasos del Análisis

1. **Preprocesamiento de Datos**
   - Eliminación de columnas redundantes (e.g., `DailyCharges`)
   - Codificación de variables categóricas con `LabelEncoder`
   - Manejo de valores faltantes en la variable objetivo

2. **Análisis Exploratorio**
   - Análisis de correlación entre variables numéricas
   - Visualizaciones de variables clave en relación a `Churn`

3. **Balanceo de Clases**
   - Uso de técnicas de undersampling, oversampling y SMOTE para equilibrar las clases

4. **Modelado**
   - Entrenamiento y evaluación de modelos: Regresión Logística, Random Forest, KNN, SVM, XGBoost
   - Comparación de desempeño con métricas como F1-score, matriz de confusión, etc.

5. **Interpretación**
   - Análisis de importancia de variables para entender qué factores afectan más la cancelación

---

## Resultados Principales

- Las variables más importantes para predecir la cancelación son: `Tenure`, `ChargesTotal`, `Contract` y `PaymentMethod`.
- Los modelos con mejor desempeño fueron Random Forest y XGBoost con un F1-score alrededor de 0.87-0.88.
- La cancelación está asociada a clientes con menor antigüedad y contratos mensuales.

---

## Recomendaciones y Estrategias de Retención

- Incentivar contratos a largo plazo para reducir churn.
- Ofrecer descuentos o promociones a clientes con baja antigüedad.
- Facilitar métodos de pago automáticos y flexibles.
- Implementar un sistema de alertas tempranas usando los modelos predictivos para detectar clientes en riesgo.

---

## Tecnologías y Librerías Utilizadas

- Python 3
- Pandas, NumPy
- scikit-learn
- imblearn (SMOTE)
- XGBoost
- Matplotlib, Seaborn

---







