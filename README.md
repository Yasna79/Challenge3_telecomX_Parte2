# Challenge3_telecomX_Parte2
 Predicción de Cancelación (Churn)
# 📊 Análisis y Predicción de Cancelación de Clientes (Churn)

---

## 🔍 Descripción

Este proyecto tiene como objetivo identificar los factores que más influyen en la cancelación de clientes y construir modelos predictivos para anticipar cuándo un cliente podría cancelar su servicio. Se utilizan técnicas de preprocesamiento, balanceo de clases y distintos modelos de machine learning para lograrlo.

---

## 🗂 Dataset

- **Archivo:** `datos_tratados.csv`  
- **Características:** Datos del cliente como duración del contrato, cargos mensuales y totales, tipo de contrato, entre otros.  
- **Variable objetivo:** `Churn` (1 = Canceló, 0 = Activo)

---

## 🛠 Proceso de Análisis

1. **Preprocesamiento**  
   - Eliminación de variables redundantes  
   - Codificación de variables categóricas  
   - Manejo de valores faltantes  

2. **Análisis Exploratorio**  
   - Matriz de correlación  
   - Visualizaciones clave (boxplots, scatter plots)

3. **Balanceo de Clases**  
   - Técnicas de undersampling, oversampling y SMOTE para balancear `Churn`

4. **Modelado**  
   - Regresión Logística, Random Forest, KNN, SVM y XGBoost  
   - Evaluación con métricas como F1-score, precisión y matriz de confusión

5. **Interpretación**  
   - Importancia de variables  
   - Análisis de coeficientes y permutation importance

---

## 📈 Resultados Clave

| Modelo              | F1 Score (Churn) | Comentarios                                   |
|---------------------|------------------|-----------------------------------------------|
| Random Forest       | ~0.88            | Excelente desempeño sin necesidad de escalado |
| XGBoost             | ~0.87            | Gran capacidad para capturar relaciones complejas |
| Regresión Logística | ~0.81            | Fácil de interpretar, buen punto de partida    |
| SVM (lineal)        | ~0.80            | Rendimiento similar a regresión logística      |
| KNN                 | ~0.75            | Más sensible al ruido y la escala               |

🔹 **Mejor modelo:** Random Forest y XGBoost por su precisión y estabilidad.

---

## 🔑 Factores que Impactan la Cancelación

- **Tenure (Antigüedad):** Clientes con menos tiempo tienen mayor riesgo de cancelar.  
- **ChargesTotal (Gasto Total):** Clientes con menor gasto total tienden a cancelar más.  
- **Contract (Tipo de contrato):** Contratos mensuales tienen mayor churn comparado con contratos a largo plazo.  
- **PaymentMethod (Método de pago):** Algunas modalidades están asociadas con mayor cancelación.

---

## 💡 Estrategias de Retención

- Incentivar contratos de mayor duración con descuentos o beneficios exclusivos.  
- Ofrecer promociones a clientes nuevos o con baja antigüedad.  
- Facilitar métodos de pago automáticos para reducir fricciones.  
- Implementar alertas tempranas con modelos predictivos para identificar clientes en riesgo.

---

## 🚀 Tecnologías Utilizadas

- Python 3  
- pandas, numpy  
- scikit-learn  
- imbalanced-learn (SMOTE)  
- xgboost  
- matplotlib, seaborn  

---



---👤 Autor
Yasna Perez Montenegro









