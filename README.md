<span class="c1"></span>

## <span class="c4">Planteamiento del Problema</span>

<span class="c4"></span>

### <span class="c20">O</span><span class="c4">bjetivo:</span>

<span class="c4"></span>

*   <span class="c1">Desarrollar y productizar un modelo predictivo para predecir el nivel de satisfacción de niños y de abuelos de acuerdo a la composición del hogar y otros determinantes.</span>

<span class="c1"></span>

### <span class="c4">Tipo de Problema:</span>

<span class="c1"></span>

*   <span class="c1">Predicción del nivel de satisfacción de niños y abuelos a partir de la composición del hogar y otros determinantes.</span>

<span class="c1"></span>

### <span class="c4">Información Disponible:</span>

<span class="c4"></span>

*   <span class="c1">El insumo principal de este trabajo son los datos de la Encuesta Nacional de Calidad de Vida - ECV 2020 (17081 registros de abuelos, 18626 registros de niños).</span>

<span class="c1"></span>

### <span class="c4">Método de Machine Learning:</span>

<span class="c1"></span>

- <span class="c1">Realización de dos modelos de regresión lineal múltiple, uno para predecir el nivel de satisfacción de niños y otro el de los abuelos siguiendo el método posterior:</span>
  -   <span class="c1">Análisis exploratorio de datos evaluando una gran cantidad de características sin hipótesis pre-especificadas para identificar y seleccionar las características que sirvan como variables predictivas.</span>
  -   <span class="c1">Ingeniería de características para construir variables predictivas del modelo.</span>
  -   <span>Modelo de regresión lineal múltiple realizado con las variables predictivas.</span><span class="c25"> </span>

<span class="c20 c25 c28"></span>

### <span class="c4">Evaluación de Métricas, Protocolo de Entrenamiento y Validación:</span>

<span class="c4"></span>

*   <span class="c1">MSE, RMSE y R-Squared serán utilizados para evaluar el rendimiento predictivo de los modelos.</span>
*   <span class="c1">13664 registros de abuelos para entrenamiento y 14900 registros de niños para entrenamiento.</span>
*   <span class="c1">3417 registros de abuelos para validación y 3726 registros de niños para validación.</span>

<span class="c1"></span>

## <span class="c4">Definiciones</span>

*   <span class="c1">Abuelo: para este trabajo se define como abuelo a la persona que es cabeza de hogar y tiene nietos, y su pareja, además de sus padres y suegros en caso de que viva con sus hijos. También es un abuelo la persona que es el padre o madre de la persona cabeza de hogar y esta persona tiene hijos, además que los suegros de esta persona son abuelos.</span>
*   <span class="c1">Niño: para este trabajo se define como niño a toda persona que tiene entre 15 y 18 años de edad.</span>

<span class="c1"></span>

## <span class="c4">Flujo de Trabajo</span>

<span class="c4"></span>

<span class="c1">A continuación se presenta el flujo de trabajo realizado:</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 601.70px; height: 666.67px;">![](images/image11.png)</span>

<span class="c5">*Figura 1*.</span> <span class="c9">Flujo de Trabajo. Fuente propia.</span>

<span class="c1"></span>

## <span class="c4">Fuentes de Datos y Preprocesamiento</span>

<span class="c4"></span>

### <span class="c4">Poblaciones:</span>

<span class="c1"></span>

*   <span class="c1">Abuelos: sujetos entre 12 y 105 años de edad de Colombia.</span>
*   <span class="c1">Niños: sujetos entre 15 y 18 años de edad de Colombia.</span>

<span class="c1"></span>

### <span class="c4">Registro de Muestra y Características de Medición:</span>

<span class="c1"></span>

*   <span class="c1">Encuesta realizada a las familias colombianas por el DANE.</span>

<span class="c1"></span>

### <span class="c4">Recopilación de Datos:</span>

<span class="c1"></span>

*   <span class="c1">Registros de abuelos y niños seleccionados de la base de datos a partir de las definiciones de abuelos y niños presentadas.</span>

<span class="c1"></span>

### <span class="c4">Estructuras de Datos y Tipos:</span>

<span class="c1"></span>

*   <span class="c1">Variables continuas seleccionadas de la base de datos.</span>
*   <span class="c1">Variables continuas creadas a partir de la ingeniería de características realizadas.</span>

<span class="c4"></span>

### <span class="c4">Preprocesamiento de Datos:</span>

<span class="c4"></span>

<span class="c1">Para los registros de los abuelos y niños:</span>

* <span class="c1">Subconjuntos de datos o agregación:</span>
  * <span class="c1">Selección de los sujetos a partir de la definición de abuelo o niño presentada.</span>
* <span class="c1">Transformación de datos:</span>
  * <span class="c1">Conversión del tipo de datos de objetos a enteros.</span>

<span class="c1"></span>

### <span class="c4">Link a la Información:</span>

<span class="c4"></span>

*   <span class="c22">[Colombia - Encuesta Nacional de Calidad de Vida - ECV 2020](https://www.google.com/url?q=https://microdatos.dane.gov.co/index.php/catalog/718/get_microdata&sa=D&source=editors&ust=1651468799389679&usg=AOvVaw0762i5vpCcXCnA1XNwGwhp)</span><span class="c1"> </span>

<span class="c1"></span>

## <span class="c4">Análisis Descriptivo</span>

<span class="c4"></span>

### <span class="c4">Análisis de datos por individuos</span>

<span class="c4"></span>

<span class="c16">Ahora se analizarán los datos de los abuelos y los niños como individuos.</span>

<span class="c1">Se observa una muestra del conjunto de datos de los niños que se analizará y un resumen de las variables cuantitativas de este:</span>

<span class="c1"></span>

<span>        </span><span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 349.00px; height: 214.00px;">![](images/image7.png)</span>

<span>        </span><span class="c5">*Figura 2*.</span> <span class="c18">Muestra de información de los niños a analizar. Fuente propia.</span>

<span>        </span><span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 188.00px; height: 315.00px;">![](images/image17.png)</span>

<span class="c5">*Figura 3*.</span> <span class="c9">Descripción de las variables cuantitativas de los niños a analizar. Fuente propia.</span>

<span class="c1"></span>

<span class="c1">        Se observa que el rango de edad de los niños es de 15 a 18 años.</span>

<span class="c1"></span>

<span class="c1">Luego se presenta una muestra del conjunto de datos de los abuelos que se analizará y un resumen de las variables cuantitativas de este:</span>

<span class="c1"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 400.00px; height: 212.00px;">![](images/image4.png)</span>

<span class="c5">*Figura 4*.</span> <span class="c18">Muestra de información de los abuelos a analizar. Fuente propia.</span>

<span class="c2"></span>

<span class="c2"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 184.00px; height: 311.00px;">![](images/image3.png)</span>

<span class="c5">*Figura 5*.</span> <span class="c9">Descripción de las variables cuantitativas de los abuelos a analizar. Fuente propia.</span>

<span class="c1"></span>

<span class="c2">Se observa que el rango de edad de los abuelos es de 16 a 105 años.</span>

<span class="c2"></span>

#### <span class="c4">Análisis de individuos por el sexo</span>

<span class="c2"></span>

<span class="c2">Seguidamente se representan los datos del sexo por medio de un gráfico de barras comparativo, donde se muestra la cantidad de niños y abuelos con sexo masculino y femenino.</span>

<span class="c2"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 510.00px; height: 470.00px;">![](images/image1.png)</span>

<span class="c5">*Figura 6*.</span> <span class="c9">Gráfico de barras comparativo de niños y abuelos por sexo. Fuente propia.</span>

<span class="c1"></span>

<span class="c2">Se nota que para los abuelos hay más mujeres que hombres mientras que para los niños las cantidades de niños y niñas son similares.</span>

<span class="c4"></span>

#### <span class="c4">Análisis de datos por la edad</span>

<span class="c4"></span>

<span class="c2">Ahora se representan los datos de edad, los cuales se dividen en edad de niños y edad de abuelos.</span>

<span class="c2"></span>

<span class="c2">Edad de los niños:</span>

<span class="c16">        </span><span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 463.00px; height: 436.00px;">![](images/image6.png)</span>

<span class="c5">*Figura 7*.</span> <span class="c9">Gráfico de barras de las edades de los niños. Fuente propia.</span>

<span class="c1"></span>

<span class="c1">Se nota que las proporciones de edades de los niños son similares.</span>

<span class="c1"></span>

<span class="c1">Edad de los abuelos:</span>

<span class="c1"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 144.00px; height: 191.00px;">![](images/image12.png)</span>

<span class="c5">*Figura 8*.</span> <span class="c9">Tabla de las edades de los niños. Fuente propia.</span>

<span class="c1"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 503.00px; height: 482.00px;">![](images/image16.png)</span>

<span class="c5">*Figura 9*.</span> <span class="c18">Gráfico de dispersión de las edades de los abuelos. Fuente propia.</span>

<span class="c1"></span>

<span>Cabe aclarar que se utilizó una gráfica diferente al gráfico de barras utilizado para las edades de los niños debido al rango de edad de los abuelos, por lo que se decidió realizar un gráfico de dispersión Edad vs. Cantidad para mostrar la cantidad de</span><span class="c23"> personas en cierto rango de edad de los abuelos. Al mirar la gráfica se observa qu</span><span class="c23 c26">e la mayoría de los abuelos se encuentran entre los 40 y los 80 años de edad.</span>

<span class="c4"></span>

#### <span class="c4">Análisis de datos según la etnia, pueblo o cultura</span>

<span class="c4"></span>

<span class="c2">Después se representan los datos de las etnias/culturas tanto de los niños como de los abuelos en un gráfico de barras comparativo.</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 463.00px; height: 742.00px;">![](images/image9.jpg)</span>

<span class="c5">*Figura 10*.</span> <span class="c18">Gráfico de barras comparativo de las etnias y culturas de los abuelos y niños. Fuente propia.</span>

<span class="c1"></span>

<span class="c2">Se aprecia que la mayoría de abuelos y niños no pertenecen a una etnia o cultura en específico y que en los datos hay muy poca representación de otras etnias y culturas.</span>

<span class="c2"></span>

<span class="c1"></span>

### <span class="c4">Análisis de datos por hogares</span>

<span class="c4"></span>

<span class="c2">Ahora se analizarán los datos de los hogares donde viven los abuelos y los niños.</span>

<span class="c2"></span>

<span class="c2">Se observa una muestra del conjunto de datos de los niños que se analizará y un resumen de las variables cualitativas de este:</span>

<span class="c2"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 293.00px; height: 196.00px;">![](images/image15.png)</span>

<span class="c5">*Figura 11*.</span> <span class="c9">Muestra de información de los hogares de los niños a analizar. Fuente propia.</span>

<span class="c9"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 344.00px; height: 162.00px;">![](images/image14.png)</span>

<span class="c5">*Figura 12*.</span> <span class="c9">Descripción de las variables cualitativas de los hogares de los niños a analizar. Fuente propia.</span>

<span class="c9"></span>

<span class="c1">Se aprecia que la gran parte de los hogares encuestados considera que están seguros, que se encuentran en la pobreza y dicen no tener internet.</span>

<span class="c2"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 353.00px; height: 194.00px;">![](images/image13.png)</span>

<span class="c5">*Figura 13*.</span> <span class="c18">Muestra de información de los hogares de los abuelos a analizar. Fuente propia.</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 391.00px; height: 168.00px;">![](images/image8.png)</span>

<span class="c5">*Figura 14*.</span> <span class="c9">Descripción de las variables cualitativas de los hogares de los abuelos a analizar. Fuente propia.</span>

<span class="c1"></span>

<span class="c2">Se observa que la mayoría de los hogares en los que residen abuelos se encuentran en condiciones similares a los hogares en los que residen los niños.</span>

<span class="c2"></span>

#### <span class="c4">Análisis de datos según sentimiento de seguridad</span>

<span class="c4"></span>

<span class="c16">Ahora se representan los datos de sentimiento de seguridad en los hogares donde residen los niños por medio de un gráfico de barras comparativo.</span>

<span class="c2"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 601.70px; height: 556.00px;">![](images/image5.jpg)</span>

<span class="c5">*Figura 15*.</span> <span class="c18">Gráfico de barras comparativo de niños y abuelos por sentimiento de seguridad.</span><span class="c18"> Fuente propia.</span>

<span class="c2"></span>

<span class="c2">Al analizar el gráfico se observa que la mayoría de hogares donde residen los abuelos y los niños se sienten seguros.</span>

<span class="c16 c24"></span>

<span class="c2"></span>

#### <span class="c4">Análisis de datos según sentimiento de pobreza</span>

<span class="c4"></span>

<span class="c2">Luego representamos los datos de sentimiento de pobreza de hogares donde residen niños y abuelos por medio de un gráfico de barras comparativo.</span>

<span class="c2"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 601.70px; height: 544.00px;">![](images/image10.jpg)</span>

<span class="c5">*Figura 16*.</span> <span class="c18">Gráfico de barras comparativo de niños y abuelos por sentimiento de pobreza. Fuente propia.</span>

<span class="c2"></span>

<span class="c2">Se aprecia que la proporción de sentimiento de pobreza es similar tanto en los hogares donde residen niños como en los hogares donde residen abuelos, predominando los hogares que sienten que están en la pobreza.</span>

<span class="c2"></span>

#### <span class="c4">Análisis de datos según la tenencia de internet</span>

<span class="c4"></span>

<span class="c2">Ahora se representan los datos sobre los hogares donde residen niños y abuelos que tienen internet.</span>

<span class="c2"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 601.70px; height: 544.00px;">![](images/image2.jpg)</span>

<span class="c5">*Figura 17*.</span> <span class="c9">Gráfico de barras comparativo de niños y abuelos por tenencia de internet. Fuente propia.</span>

<span class="c9"></span>

<span class="c16">Se nota que hay más hogares donde residen niños sin internet que hogares donde residen abuelos, y se nota una proporción similar en ambos casos.</span>

<span class="c4"></span>

## <span class="c4">Desarrollo de los Modelos y Validación</span>

### <span class="c4">Software Utilizado:</span>

<span class="c1"></span>

*   <span>Modelos realizados en</span> <span class="c22">[Google Collaboratory](https://www.google.com/url?q=https://colab.research.google.com/notebooks/welcome.ipynb?hl%3Des&sa=D&source=editors&ust=1651468799400076&usg=AOvVaw3BsmzIFA0LLERerLBE2zcG)</span><span> con el lenguaje de programación Python utilizando la librería</span> <span class="c22">[Sklearn](https://www.google.com/url?q=https://scikit-learn.org/stable/&sa=D&source=editors&ust=1651468799400362&usg=AOvVaw23RUSQiQ8kNy3KoPx_MyLq)</span><span class="c1">.</span>

<span class="c1"></span>

### <span class="c4">Entrenamiento y Validación de los Modelos:</span>

<span class="c1"></span>

*   <span class="c1">Entrenamiento completado utilizando 13664 registros de abuelos y 14900 registros de niños.</span>

<span class="c1"></span>

### <span class="c4">Características Seleccionadas y Entrada a los Modelos:</span>

<span class="c4"></span>

<span class="c1">Las características se seleccionaron teniendo en cuenta la revisión de literatura que se realizó previa al desarrollo de los modelos que permitió llevar a cabo  la ingeniería de características y con base en la evaluación de la correlación de las variables que ya se presentaban en la base de datos.</span>

<span class="c1"></span>

*   <span class="c1">Para el modelo de los abuelos: 'step_in_life', 'free_time_satisfaction', 'health_satisfaction', 'happiness_yesterday', 'life_worthiness', 'job_satisfaction', 'safety_satisfaction', 'worried_level', 'sadness_level', 'home_life_conditions', 'childhouse_home', 'home_incomes', 'kids_amount', 'teenagers_amount', 'sons_amount', 'has_partner'.</span>
*   <span class="c1">Para el modelo de los niños: 'step_in_life', 'free_time_satisfaction', 'health_satisfaction', 'happiness_yesterday', 'life_worthiness', 'life_satisfaction', 'safety_satisfaction', 'worried_level' 'sadness_level', 'home_life_conditions', 'childhouse_home', 'has_internet', 'poverty', 'live_after_5_years'.</span>

<span class="c1"></span>

### <span class="c4">Variable a Predecir y Salida de los Modelos:</span>

<span class="c1"></span>

*   <span>Al realizar el análisis exploratorio en la base de datos se identificó que la variable</span> <span class="c20">‘life_satisfaction’</span><span class="c1"> permite demostrar el nivel de satisfacción de niños y de abuelos de acuerdo a las características seleccionadas, por lo cual, se escogió como variable a predecir tanto para niños como para abuelos.</span>

<span class="c1"></span>

### <span class="c4">Método de Validación:</span>

<span class="c1"></span>

*   <span class="c1">Validación realizada utilizando 3417 registros de abuelos y 3726 registros de niños.</span>

<span class="c1"></span>

### <span class="c4">Reproducibilidad y Reutilización del Código:</span>

<span class="c1"></span>

* <span class="c1">Modelos para niños y abuelos:</span>
  * <span class="c22">[código fuente en Google Colab](https://www.google.com/url?q=https://colab.research.google.com/drive/16ONg9wMgshDy7LWFBoMfQunBwa7dj6cN?usp%3Dsharing&sa=D&source=editors&ust=1651468799402566&usg=AOvVaw0tWC-t0il-rrEOolSu0QME)</span>
  * <span class="c22">[código fuente en Github](https://www.google.com/url?q=https://github.com/CloaizaF/Trabajo_TAE_1&sa=D&source=editors&ust=1651468799402863&usg=AOvVaw31tac89dtWBVZVogcProDa)</span>

* <span class="c1">Modelos para niños y abuelos en producción:</span>
  * <span class="c22">[back end](https://www.google.com/url?q=https://github.com/jumarinr/satisfaccion_model&sa=D&source=editors&ust=1651468799403202&usg=AOvVaw3pevcbDMtaaZVaWmw5dmLJ)</span>
  * <span class="c22">[front end](https://www.google.com/url?q=https://github.com/jumarinr/prediction-satisfaction&sa=D&source=editors&ust=1651468799403461&usg=AOvVaw3QCVXGL6IQglMXrpFoWwiZ)</span>

<span class="c4"></span>

## <span class="c4">Modelo en Producción</span>

<span class="c4"></span>

*   <span class="c22">[Link a la aplicación web](https://www.google.com/url?q=https://prediction-satisfaction.herokuapp.com/&sa=D&source=editors&ust=1651468799403947&usg=AOvVaw0PChPHa0Ek07fy4ydWjeIk)</span>

<span class="c1"></span>

## <span class="c4">Video Promocional</span>

<span class="c4"></span>

*   <span class="c22">[Link al video promocional](https://www.google.com/url?q=https://www.youtube.com/watch?v%3D1mPLnMfjhQg%26feature%3Dyoutu.be&sa=D&source=editors&ust=1651468799404484&usg=AOvVaw1it3N2rSRbObLFzEvM979f)</span>

<span class="c1"></span>

## <span class="c4">Conclusiones</span>

<span class="c4"></span>

*   <span>Como conclusión del trabajo cabe resaltar que la estimación de algo tan subjetivo como lo es la satisfacción con la vida de alguien es bastante retador  de acotar usando criterios aunque estos estén fundamentados con estudios, principalmente por la heterogeneidad de los grupos estudiados; sin embargo, gracias al análisis exploratorio se pudo asociar la satisfacción con la vida con varias de las preguntas que se realizaron en la encuesta,</span> <span class="c2">estas tenían que ver principalmente con lo cómodo que se encontraban los encuestados con su tiempo libre, seguridad, empleo, entre otras.</span>
*   <span class="c2">Por otra parte la gran parte de las variables que se crearon haciendo uso de la ingeniería de características tuvieron poca correlación con la variable a predecir, futuros estudios deben realizarse con el fin de encontrar mejores  criterios.</span>
*   <span class="c16">Con respecto a las métricas usadas para evaluar la predicción del modelo se puede notar que el usado para abuelos es un poco menos preciso que el modelo para niños, esto puede comprobarse por ejemplo, al observar el error cuadrático medio de ambos modelos, siendo de 1.70 y 1.22 respectivamente, esto es debido a que las variables usadas para el modelo de los niños presentan una mayor correlación que los abuelos en la gran mayoría de la variables seleccionadas, esto se evidencia ya que se obtuvo un</span> <span class="c11 c16">R^2 de</span> <span class="c2">0.48 y 0.54 para abuelos y niños respectivamente.</span>

<span class="c2"></span>

## <span class="c4">Referencias</span>

<span class="c4"></span>

<span>Gadermann, A. M., Guhn, M., & Zumbo, B. D. (2010). Investigating the Substantive Aspect of Construct Validity for the Satisfaction with Life Scale Adapted for Children: A Focus on Cognitive Processes.</span> <span class="c11">Social Indicators Research</span><span>,</span> <span class="c11">100</span><span>(1), 37–60\.</span> <span class="c22">[https://doi.org/10.1007/s11205-010-9603-x](https://www.google.com/url?q=https://doi.org/10.1007/s11205-010-9603-x&sa=D&source=editors&ust=1651468799406033&usg=AOvVaw210DIzqFUHA600OU_K-x5h)</span>

<span class="c1"></span>

<span>Migliorini, L., Tassara, T., & Rania, N. (2018). A Study of Subjective Well-Being and Life Satisfaction in Italy: how are Children doing at 8 years of Age?</span> <span class="c11">Child Indicators Research</span><span>,</span> <span class="c11">12</span><span>(1), 49–69\.</span> <span class="c22">[https://doi.org/10.1007/s12187-017-9514-3](https://www.google.com/url?q=https://doi.org/10.1007/s12187-017-9514-3&sa=D&source=editors&ust=1651468799406507&usg=AOvVaw3PAlBy7GTWz3Fc_45zPpGC)</span>

<span class="c1"></span>

<span>Ní Mhaoláin, A. M., Gallagher, D., O Connell, H., Chin, A. V., Bruce, I., Hamilton, F., Teehee, E., Coen, R., Coakley, D., Cunningham, C., Walsh, J. B., & Lawlor, B. A. (2011). Subjective well-being amongst community-dwelling elders: what determines satisfaction with life? Findings from the Dublin Healthy Aging Study.</span> <span class="c11">International Psychogeriatrics</span><span>,</span> <span class="c11">24</span><span>(2), 316–323\.</span> <span class="c22">[https://doi.org/10.1017/s1041610211001360](https://www.google.com/url?q=https://doi.org/10.1017/s1041610211001360&sa=D&source=editors&ust=1651468799406986&usg=AOvVaw2qAGU_Wo4_MqGzW2Lre_i7)</span>

<span class="c1"></span>

<span>Ranzijn, R., & Luszcz, M. (2000). Measurement of Subjective Quality of Life of Elders.</span> <span class="c11">The International Journal of Aging and Human Development</span><span>,</span> <span class="c11">50</span><span>(4), 263–278\.</span> <span class="c22">[https://doi.org/10.2190/4b0w-amgu-2ndx-cyuq](https://www.google.com/url?q=https://doi.org/10.2190/4b0w-amgu-2ndx-cyuq&sa=D&source=editors&ust=1651468799407426&usg=AOvVaw0A8989ok0LqAn6qh7pG_fr)</span>

<span class="c1"></span>

<span>Stevens, L. M., Mortazavi, B. J., Deo, R. C., Curtis, L., & Kao, D. P. (2020). Recommendations for Reporting Machine Learning Analyses in Clinical Research.</span> <span class="c11">Circulation: Cardiovascular Quality and Outcomes</span><span>,</span> <span class="c11">13</span><span>(10).</span> <span class="c22">[https://doi.org/10.1161/circoutcomes.120.006556](https://www.google.com/url?q=https://doi.org/10.1161/circoutcomes.120.006556&sa=D&source=editors&ust=1651468799407887&usg=AOvVaw0onRU2FrbcwyLcoXjah9Eb)</span><span> </span>

<span class="c1"></span>

<span class="c20">        </span>

<div>

<span class="c1"></span>

</div>
