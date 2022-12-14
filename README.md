# <h1 align="center">**`PI02_DATA05`**
# <h1 align="center">**`Segundo Proyecto Individual - Machine Learning `**
# <h1 align="center">**`María Belén Sendot`**

<p align="center">
<img src="https://img.freepik.com/vector-premium/hospitalizacion-paciente_7737-1774.jpg?w=900"   
>
</p>

​
¡Bienvenidos a mi Segundo Proyecto de Data Science! En esta ocasion estuve poniendo en práctica mis habilidades en el campo de la predicción. El objetivo del siguiente trabajo fue probar diferentes modelos de Machine Learning para encontrar aquel que pudiera darme la mejor predicción en cuanto a la problemática planteada.
​

## 🏥 **Estancia hospitalaria** 🏥

La hospitalización, o estancia hospitalaria, cuando es prolongada constituye una preocupación a nivel mundial debido a sus efectos negativos en el sistema de salud, aumentando los costos, generando deficiencia en la accesibilidad de prestación de servicios de salud, saturación de unidades de hospitalización y urgencias, por consiguiente, mayores efectos adversos como lo son las enfermedades intrahospitalarias.

El estudio de los procesos de atención en salud, así como el conocimiento de las características y perfiles de los usuarios con el objetivo de predecir la ocupación hospitalaria, es uno de los aspectos al que las autoridades de salud han prestado gran interés, pues permite no sólo garantizar los recursos necesarios para la atención del paciente, sino realizar ajustes respecto a la oferta y demanda de los servicios de salud y los implementos asociados.
​
## **Descripción del problema**

Un importante Centro de Salud lo ha contratado con el fin de poder predecir si un paciente tendrá una estancia hospitalaria prolongada o no, utilizando la información contenida en el dataset asociado, la cual recaba una muestra histórica de sus pacientes, para poder administrar la demanda de camas en el hospital según la condición de los pacientes recientemente ingresados. 

Para esto, se define que un paciente posee estancia hospitalaria prolongada si ha estado hospitalizado más de 8 días. Por lo que debe generar dicha variable categórica y luego categorizar los pacientes según las variables que usted considere necesarias, justificando dicha elección. 
​
## **Entrega**
​
El presente repositorio contiene el código en un script .py o Jupyter Notebook .ipynb, el cual incluye un EDA, feature engineerging y un pipeline de Machine Learning para el procesamiento de datos. En el mismo se **explica claramente cada paso realizado** mediante comentarios en el script y textos formato markdown dentro del Notebook.
​
A su vez, posee un script que genero un archivo .csv sólo con las predicciones, teniendo únicamente **una sola columna** (sin index) y que contiene todos los valores de las predicciones, con un valor por fila. 
​
## **Análisis y Resolucion del Problema**
​
Como observamos en la consigna, el problema consistía en poder predecir del mejor modo cual podría llegar a ser la ocupacion hospitalaria ya sea a corto o largo plazo con los nuevos datos ingresados.
Para realizar esta prediccion probe tres modelos distintos de Machine Learning (Regresión Logística, K-Vecinos y Arboles de decición) realizando un testeo con las metricas de Accuracy y Recall, para evaluar cual daba mejores resultados. La conclución fue que el mejor modelo para este tipo de datos, teniendo en cuenta la informacion de la columna Stay y en correlacion con las columnas de edad, género y departamento (las que estudié que estaban mejor correlacionadas), es el de ´Arbol de Desición´ con una profundidad de 4 capas.
El Notebook incluye anotaciones con la explicacion de cada uno de los pasos realizados y la evaluación del modelo tambien a partir de la matriz de confusión.
  
Una vez elegido el modelo, procedí a realizar el Pipeline del mismo para empaquetarlo, disponibilizarlo para su uso, y exporté la columna con las predicciones de mi modelo en un archivo csv.

<p align="center">
<img src="https://valohai.com/assets/img/manual-pipeline.png"   
>
</p>
