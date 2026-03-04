# MNIST - Clasificación de Dígitos con Regresión Logística

Este proyecto consiste en un análisis completo del dataset MNIST, utilizando Python y scikit-learn para construir un modelo de clasificación capaz de reconocer dígitos escritos a mano.

El notebook incluye desde la exploración inicial de los datos hasta el entrenamiento y evaluación de modelos tanto binarios como multiclase.

---

## Objetivos del proyecto

* Comprender la estructura del dataset MNIST.
* Realizar análisis exploratorio de imágenes.
* Visualizar la distribución de clases.
* Implementar un modelo de clasificación binaria (detección del número 5).
* Implementar un modelo de clasificación multiclase.
* Evaluar el rendimiento usando métricas como accuracy, precision, recall y F1-score.
* Interpretar correctamente los resultados en contextos desbalanceados.

---

## Dataset

Se utiliza el dataset MNIST, compuesto por imágenes de:

* 28x28 píxeles en escala de grises
* 784 características por muestra (imagen aplanada)
* 70.000 imágenes en total
* 10 clases (dígitos del 0 al 9)

---

## Estructura del notebook

### 1. Carga de datos

Se cargan las imágenes y sus etiquetas, separando:

* `x` → características (píxeles)
* `y` → etiquetas (dígito correspondiente)

---

### 2. Visualización de imágenes

* Se muestran imágenes aleatorias del dataset.
* Se reconstruyen las matrices 28x28 a partir de los vectores de 784 dimensiones.
* Se genera una visualización promedio por clase (centroide de cada dígito).

Esto permite entender la variabilidad y estructura espacial de los datos.

---

### 3. Análisis de distribución

Se genera un gráfico de barras para observar la cantidad de muestras por clase, detectando posibles desbalances.

---

### 4. Clasificación binaria (detección del número 5)

Se entrena un modelo de regresión logística para responder:

> ¿Es este dígito un 5 o no?

Se analizan métricas como:

* Precision
* Recall
* F1-score
* Support

Se discute la diferencia entre accuracy y rendimiento real en clases desbalanceadas.

---

### 5. Clasificación multiclase

Se entrena un modelo de regresión logística para clasificar directamente los 10 dígitos.

Incluye:

* División train/test
* Escalado con StandardScaler
* Entrenamiento del modelo
* Evaluación del rendimiento

---

## Tecnologías utilizadas

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* scikit-learn

---

## Métricas de evaluación

Se utilizan métricas estándar de clasificación:

* Accuracy
* Precision
* Recall
* F1-score
* Matriz de confusión

Se analiza especialmente el comportamiento en clases minoritarias.

---

## Aprendizajes clave

* Cómo representar imágenes como vectores en espacios de alta dimensión.
* Importancia del escalado en modelos lineales.
* Diferencia entre clasificación binaria y multiclase.
* Impacto del desbalance de clases en la interpretación de métricas.
* Interpretación geométrica del centroide de clase en espacios de 784 dimensiones.

  ---
  El objetivo es desarrollar una APK que reconozca digitos por fotografía. 

