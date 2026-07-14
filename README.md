# Educación y Trabajo Decente: Análisis Exploratorio de Indicadores ODS

##  Descripción del Proyecto
Trabajo Práctico Integrador desarrollado para la materia **Laboratorio de Datos II (1°C 2026)** de la **Universidad CAECE**. 

El proyecto consiste en un Análisis Exploratorio de Datos (EDA) que busca responder a la pregunta de si existe una relación directa entre la mejora de los indicadores educativos de un país y sus condiciones laborales y económicas. 

Para esto, se analizaron datos oficiales de las Naciones Unidas correspondientes a:
* **ODS 4 (Educación de Calidad):** Alfabetización, Finalización educativa y Participación en educación.
* **ODS 8 (Trabajo Decente y Crecimiento Económico):** Tasa de desempleo, Jóvenes NEET (que no estudian ni trabajan) y Crecimiento del PIB per cápita.

##  Arquitectura y Datos
A diferencia de los análisis estáticos tradicionales, este proyecto implementa una arquitectura moderna de datos:
1. **Extracción:** Consumo de datos crudos mediante la API oficial de Naciones Unidas.
2. **Almacenamiento:** Persistencia de más de 196.000 documentos en una base de datos NoSQL utilizando **MongoDB Atlas**.
3. **Procesamiento:** Conexión, limpieza, filtrado (BOTHSEX + ALLAREA) y análisis mediante Python en Jupyter Notebooks.

##  Principales Conclusiones (Negocio)
Tras analizar el periodo 2000-2023 a nivel mundial, la hipótesis se cumplió de manera parcial:
* **Relación Clara:** Se observó una correlación negativa moderada ($r = -0.52$) entre la finalización educativa y los jóvenes NEET. A mayor nivel educativo, menor es la tasa de jóvenes que no estudian ni trabajan.
* **El factor económico:** La relación de la educación con el desempleo es mucho más débil. El acceso al empleo no depende únicamente de la formación, sino de la coyuntura económica de cada país (visibilizado fuertemente en la fuerte caída global del PIB per cápita durante la pandemia en 2020).

##  Stack Tecnológico
* **Lenguaje:** Python
* **Base de Datos:** MongoDB Atlas (PyMongo)
* **Manipulación de Datos:** Pandas, NumPy
* **Visualización:** Matplotlib, Seaborn

##  Estructura del Repositorio
* `/notebooks`: Contiene el Jupyter Notebook (`notebook.ipynb`) con el proceso de conexión a MongoDB, limpieza y gráficos de correlación.
* `/reports`: Incluye la presentación ejecutiva del proyecto en PDF (`presentacion_ods.pdf`).

##  Integrantes del Proyecto
* Cardona, Santiago
* Díaz, Noelia
* Frati, Gianluca
* Suárez, Dante
