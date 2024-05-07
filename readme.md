![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Laboratorio | Datos desequilibrados

Usaremos el conjunto de datos `files_for_lab/customer_churn.csv` para crear un predictor de abandono.

### Instrucciones

1. Cargue el conjunto de datos y explore las variables.
2. Intentaremos predecir la variable "Churn" utilizando una regresión logística sobre las variables "tenure", "SeniorCitizen", "MonthlyCharges".
3. Extraiga la variable de destino.
4. Extraiga las variables independientes y escalelas.
5. Construya el modelo de regresión logística.
6. Evaluar el modelo.
7. Incluso un modelo simple nos dará más del 70% de precisión. ¿Por qué?
8. **La técnica de sobremuestreo de minorías sintéticas (SMOTE)** es una técnica de sobremuestreo basada en vecinos más cercanos que agrega nuevos puntos entre puntos existentes. Aplique `imblearn.over_sampling.SMOTE` al conjunto de datos. Construir y evaluar el modelo de regresión logística. ¿Hay alguna mejora?
9. **Enlaces Tomek** son pares de instancias muy cercanas, pero de clases opuestas. Eliminar las instancias de la clase mayoritaria de cada par aumenta el espacio entre las dos clases, facilitando el proceso de clasificación. Aplique `imblearn.under_sampling.TomekLinks` al conjunto de datos. Construir y evaluar el modelo de regresión logística. ¿Hay alguna mejora?