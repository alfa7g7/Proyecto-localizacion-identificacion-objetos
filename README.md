# Proyecto-localizacion-identificacion-objetos
---
# **Fundamentos-analitica-II**
FACULTAD DE INGENIERÍA, DISEÑO Y CIENCIAS APLICADAS

MAESTRÍA EN CIENCIA DE DATOS

TIC 60153 – Fundamentos de analítica II

*PROYECTO DE IDENTIFICACION Y LOCALIZACION DE OBJETOS*

GRUPO:
- Esteban Ordoñez
- Raul Echeverry
- Fabian Salazar Figueroa
---


### **Description**:
Se requiere desarrollar un modelo predictivo que tiene que determinar la clasificación y localización de Pinguinos o Tortugas que aparecen en una imagen. Se le proporciona un conjunto de datos que contiene imágenes y sus anotaciones correspondientes. Su modelo debe detectar qué animal es y la ubicación en la foto.

### **Evaluation**

- #### CNN personalizado:
Cree un modelo de red neuronal convolucional personalizado como backbone (features extractor) y entrénelo desde cero (1,5 puntos)

- #### Predicción del cuadro delimitador (Bounding box):
Implemente una cabeza de regresión que se alimenta con las características extraídas del backbone convolucional. (1 punto)

- #### Clasificación de objetos:
Implementar una cabeza de clasificación que se alimenta con las características extraídas del backbone convolucional (1 punto)

- #### Aumento de datos (Data Augmentation):
Compara el uso de diferentes técnicas de aumento de datos para ver su impacto en el desempeño de ambas tareas (clasificación y regresión) (0,5 puntos)

- #### Transferir aprendizaje (Transfer learning):
Usar dos modelos preentrenados como backbones y conectar los creados previamente cabezas de clasificación y regresión para recibir entradas de ellas. (1 punto)


### **Competencia**

Adicionalmente, al tratarse de una competencia, según la posición en la misma se otorgarán puntos de bonificación de la siguiente manera:

- Primer grupo: 1 punto

- Segundo grupo: 0.6 puntos

- Tercer grupo: 0.3 puntos

Tengan en cuenta que deben seguir un protocolo correcto de evaluación para evitar la fuga de datos de los conjuntos de prueba en los pasos de procesamiento de datos. Los errores serán sancionados (-0,5 puntos cada uno). La métrica de evaluación para esta competencia es el coeficiente de dados para la tarea de regresión de cuadro delimitador y accuracy para la tarea de clasificación de objetos.

### **Submission**

Para cada conjunto de técnicas en el dataset, los submission deben contener las siguientes columnas:

- filename,class_id
- image_id_000_.jpg,1
- image_id_001_.jpg,2
- image_id_002_.jpg,2
- etc.

### **Citation**

- Daniel Osorio and JavierDiaz. AF II 2024-II: object localization. https://kaggle.com/competitions/af-ii-2024-ii-object-localization, 2024. Kaggle.

- @misc{af-ii-2024-ii-object-localization,
    author = {Daniel Osorio and JavierDiaz},
    title = {AF II 2024-II: object localization},
    year = {2024},
    howpublished = {\url{https://kaggle.com/competitions/af-ii-2024-ii-object-localization}},
    note = {Kaggle}
}
