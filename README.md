### Proyecto de Clusterización de Clientes
#### Sobre el Proyecto
Este proyecto simula un problema de negocio ficticio utilizando datos públicos del Kaggle. El objetivo principal es segmentar clientes a través de sus patrones de comportamiento y personalidad, utilizando técnicas de análisis de datos y machine learning no supervisado.

#### Herramientas y Métodos Utilizados
**Lenguaje:** Python  
**Principales bibliotecas:** Pandas, Matplotlib, Seaborn, Scikit-learn  
**Entornos:** Jupyter Notebook (para desarrollo), VSCode (para documentación)  
**Control de versiones:** Git y GitHub 

**Metodologías aplicadas:**
- Análisis exploratorio de datos (EDA)
- Ingeniería de características (Feature Engineering)
- Método del Codo (Elbow Method)
- Algoritmo de clustering K-Means

#### Problema de Negocio
Una nueva tienda enfrenta dificultades para segmentar a sus clientes según sus características personales, lo que complica el desarrollo de campañas de marketing eficaces y personalizadas.

La empresa desea identificar patrones de comportamiento y preferencias con el fin de crear segmentos de mercado más precisos y efectivos.

#### Enfoque Estratégico
El proyecto busca agrupar a los clientes en distintos segmentos en función de su comportamiento y estilo de vida. A través de algoritmos de clusterización, se obtienen grupos que permiten desarrollar estrategias de marketing personalizadas, orientadas a las necesidades y preferencias de cada segmento.

#### Descripción de los Datos  
**Columna	Descripción**  
**ID-** Identificador del cliente  
**Year_Birth-** Año de nacimiento del cliente  
**Education-** Nivel educativo  
**Marital_Status-**	Estado civil  
**Income-**	Ingreso anual del hogar  
**Kidhome-**	Número de niños en el hogar  
**Teenhome-**	Número de adolescentes en el hogar  
**Dt_Customer-**	Fecha de registro del cliente  
**Recency-**	Días desde la última compra  
**Complain-**	Quejas en los últimos 2 años (1: sí, 0: no)  
**MntWines-**	Gasto en vinos  
**MntFruits-**	Gasto en frutas  
**MntMeatProducts-**	Gasto en carne  
**MntFishProducts-**	Gasto en pescados  
**MntSweetProducts-**	Gasto en dulces  
**MntGoldProds-**	Gasto en productos de lujo  
**AcceptedCmp1 a Cmp5-**	Respuestas a campañas promocionales  
**Response-**	Respuesta a la última campaña  
**NumDealsPurchases-**	Compras con descuento  
**NumCatalogPurchases-**	Compras por catálogo  
**NumStorePurchases-**	Compras en tienda física  
**NumWebPurchases-**	Compras por el sitio web  
**NumWebVisitsMonth-**	Visitas al sitio web en el último mes  

#### Etapas del Proyecto
- Tratamiento y análisis de los datos: Se realizó limpieza, transformación e ingeniería de características. Se derivaron columnas como TotalAmountSpent (gasto total) y TotalPurchases (número total de compras).
- Asignación de pesos a variables importantes.
- Selección del número óptimo de clústeres utilizando el método del codo (Elbow).
- Algoritmo utilizado: K-Means.

(Próximamente): Aplicación de silhouette_score para mejorar la evaluación de los clusters.

#### Segmentación Final
Se identificaron 4 clusters con los siguientes perfiles:

**Cluster 0**
Menor gasto total y ticket promedio.
Buena respuesta a promociones.
Renta más baja, con algunos outliers.
Mayor número de hijos.
Clientes recientes, mayor uso del sitio web.

**Cluster 1**
Clientes de alto valor: mayor gasto y ticket promedio.
Compran más a precio regular que con descuento.
Mayor ingreso familiar.
Compran por catálogo, menos visitas al sitio.
Clientes antiguos, pocos hijos.

**Cluster 2**
Gasto moderado (aproximadamente la mitad de Cluster 1).
Ticket promedio intermedio.
Aprovechan menos promociones.
Segunda mayor renta, también antiguos.

**Cluster 3**
Bajo gasto y ticket promedio ligeramente superior a Cluster 0.
Alta respuesta a promociones.
Baja renta, muchas visitas web.
Mayor número de hijos, tiempo largo sin comprar (posible churn).

#### Consideraciones Finales
Este análisis proporciona información valiosa para apoyar a los equipos de marketing en la toma de decisiones estratégicas. La segmentación obtenida puede guiar campañas personalizadas, aumentar la retención de clientes y mejorar la rentabilidad del negocio.

Este proyecto está bajo la Licencia MIT. Consulta el archivo LICENSE para más detalles.
