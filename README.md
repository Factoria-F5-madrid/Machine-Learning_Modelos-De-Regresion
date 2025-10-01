# Modelos de Regresión en Machine Learning

## 📝 Descripción del Proyecto

Este repositorio documenta los fundamentos, los principales algoritmos y las métricas de evaluación esenciales para los problemas de **Regresión** dentro del campo del Machine Learning (Aprendizaje Automático).

Los modelos de regresión son una forma de aprendizaje supervisado utilizados para predecir un valor de salida continuo (numérico) basándose en una o más variables de entrada (características).

## 🚀 Conceptos Fundamentales

### ¿Qué es la Regresión?

La regresión en Machine Learning es una tarea que modela la relación entre variables para predecir un resultado continuo, a diferencia de la clasificación, que predice una etiqueta discreta (categoría).

| Característica | Regresión | Clasificación |
| :--- | :--- | :--- |
| **Tipo de Predicción** | Valor continuo (e.g., precio, temperatura) | Etiqueta discreta (e.g., spam/no spam, gato/perro) |
| **Objetivo** | Predecir un valor numérico exacto. | Asignar una categoría o clase. |
| **Ejemplo** | Predecir el precio de una casa. | Determinar si una transacción es fraudulenta. |

---

## 🔬 Tipos de Algoritmos de Regresión

Existen diversos modelos para abordar problemas de regresión, cada uno adecuado para diferentes tipos de relaciones en los datos:

### 1. Regresión Lineal

Busca establecer una relación lineal entre la variable independiente ($X$) y la variable dependiente ($Y$).

* **Regresión Lineal Simple:** Una sola variable independiente.
    $$Y = \beta_0 + \beta_1 X + \epsilon$$
* **Regresión Lineal Múltiple:** Múltiples variables independientes.
    $$Y = \beta_0 + \beta_1 X_1 + \beta_2 X_2 + \dots + \beta_n X_n + \epsilon$$

### 2. Regresión Polinomial

Se utiliza cuando la relación entre las variables no es lineal. En lugar de una línea recta, el modelo ajusta una curva a los datos, elevando la variable independiente a diferentes potencias ($X^2, X^3$, etc.).

### 3. Regresión Regularizada (Regularization)

Técnicas utilizadas para prevenir el sobreajuste (*overfitting*) penalizando los coeficientes grandes.

* **Regresión Ridge (L2):** Añade una penalización basada en el cuadrado de los coeficientes ($\sum \beta^2$). Esto reduce la magnitud de los coeficientes, pero no los lleva a cero.
* **Regresión Lasso (L1):** Añade una penalización basada en el valor absoluto de los coeficientes ($\sum |\beta|$). Puede llevar algunos coeficientes a cero, realizando una **selección automática de características**.
* **Elastic Net:** Combina las penalizaciones L1 y L2 (Ridge y Lasso).

### 4. Modelos Basados en Árboles

* **Regresión con Árboles de Decisión:** Divide el espacio de características en regiones simples y predice el promedio (o mediana) del objetivo para los puntos en cada región.
* **Bosques Aleatorios para Regresión:** Combina las predicciones de múltiples árboles de decisión para mejorar la precisión y reducir la varianza.

---

## 📊 Métricas de Evaluación

Para evaluar el rendimiento de un modelo de regresión, se utilizan varias métricas clave que miden la diferencia entre los valores predichos ($\hat{y}$) y los valores reales ($y$).

| Métrica | Fórmula | Descripción |
| :--- | :--- | :--- |
| **Error Absoluto Medio (MAE)** | $$\frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i|$$ | Es el promedio de los errores absolutos. Es robusto a los *outliers*. |
| **Error Cuadrático Medio (MSE)** | $$\frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2$$ | Promedio de los errores al cuadrado. Penaliza fuertemente los errores grandes. |
| **Raíz del Error Cuadrático Medio (RMSE)** | $$\sqrt{\frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2}$$ | La raíz cuadrada del MSE. Mantiene las unidades originales de la variable objetivo, facilitando la interpretación. |
| **Coeficiente de Determinación ($R^2$)** | $$1 - \frac{\text{MSE}}{\text{Varianza total}}$$ | Indica la proporción de la varianza en la variable dependiente que es predecible a partir de las variables independientes. Un valor más cercano a 1 es mejor. |

---
## 🛠 Enlaces Disponibles

* https://gamma.app/docs/Machine-learning-Tipos-de-regresion-roelhxblmlu3ze0?mode=doc
* https://www.canva.com/design/DAGzoM6OnVQ/In81i49kcBr1NS-TgQkXjQ/edit
* https://www.canva.com/design/DAGzpTRlPUo/g4WS08fdrcURljo2wfsmqw/edit
---

## 🛠 Tecnologías y Dependencias Sugeridas

Este tipo de proyectos típicamente se implementan usando:

* **Lenguaje:** Python
* **Librerías de ML:** Scikit-learn, Statsmodels
* **Manejo de Datos:** Pandas, NumPy
* **Visualización:** Matplotlib, Seaborn

```bash
# Entorno virtual y dependencias
pip install pandas numpy scikit-learn matplotlib seaborn
