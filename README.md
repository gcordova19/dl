# Práctica final del módulo de Deep Learning
Utilizando el dataset airbnb-listings.csv se ha utilizado los datos tabularess y las imagenes en distintos modelos de DL, de esta forma se consigue combinar distintos tipos de datos. En esta tarea todos los cuadernos intentan solusionar esta tarea usando Regresion. Nota: En estea tarea los labels no se transformaron.

# Distribucion del trabajo.

Se presentan 5 cuadernos Jupyter

- downloadData.ipynb: Contiene el preprosesado del dataset y la descarga de imagenes.No se ha selecionado las variables recomendadas de interes por que se uso la exploracion anterior al modulo.

- modelado1.ipynb: Usando solo datos tabulares se aplican distintas arquitecturas desde cero y ademas se aplican tecnicas de eliminacion de Overfiting y Optimización de hiperparámetros. Se utilizaron las técnicas de regularización, como la regularización L1/L2 y la eliminación de características (dropout).
Ejecucion de diversas pruebas. Respecto a los resultados se ha podido ver que algunos modelos tenian complejidad excesiva, los modelos tienen una capacidad excesiva en comparación con el tamaño y la complejidad del conjunto de datos tabulares.

- modelado2.ipynb: usando solo imagnes se utiliza features extracture con ResNet50 (modelo pre entrenado) y a continuacion un capas densas para obtener la regresion del precio. Uso de transferlearning/ fine-tuning

- modelado3.ipynb: Se utiliza una arquitectura sencilla para presentar los conceptos Early-fusion y Late-fusion. 

- modeladoExtra.ipynb: Modificacion del tutorial https://www.pyimagesearch.com/2019/02/04/keras-multiple-inputs-and-mixed-data/ para combinar los datos tabulares e imagenes con el fin de calcular el precio.

Los resultados obtenidos pueden ser debido al uso de características irrelevantes ,los modelos pueden aprender patrones incorrectos o sesgados que no se generalizan bien a nuevos datos. La larga espera entre ejecuciones del uso gratuido de Colab ha hecho que sea dificil encontrar hiperparámetros adecuados. Los hiperparámetros del modelo, como la tasa de aprendizaje, el tamaño del lote, el número de capas y neuronas, pueden influir en el rendimiento del modelo. Si estos hiperparámetros no están ajustados adecuadamente, el modelo puede sufrir de sobreajuste.

Posibles mejoras: Aumentar el tamaño del conjunto de datos usando DataAumentation, mejorar el análisis de características para identificar y eliminar características irrelevantes o ruidosas. Se podria aplicar una validación cruzada adecuada para evaluar el rendimiento del modelo de manera más robusta.
Configurar un PC local para ajustar los hiperparámetros poder lanzar distintas ejecuciones sin problemas con colab con el fin de que mediante la búsqueda de hiperparámetros mejorar las predicciones.