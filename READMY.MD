Aplicación n-gramas: generación de frases «mañaneras»


Instrucciones
El objetivo de este mini-task es hacer un generador de texto usando como conjunto de dados entrenamiento las controvertidas conferencias matutinas de el Presidente Andrés Manuel López Obrador, sin duda sin precedente en la vida política del país. Las indicaciones específicas son las siguientes:

El líder del equipo debe de repartir, en base al conocimiento y habilidades de los miembros del equipo diferentes tareas para lograr el objetivo. Se deben exportar e incluir las libretas en html. Al final, cada equipo hará una presentación de 10 minutos de los resultados obtenidos.

LIBRETA 1: obtención de datos
A partir de los datos de las conferencias de https://github.com/NOSTRODATA/conferencias_matutinas_amlo (favor de hacer la cita y dar los créditos correspondientes) construir un corpus llamado conferencias_matutinas_amlo.txt 
Hacer una descripción breve del procedimiento específico que se llevó a cabo para armar el corpus. 
LIBRETA 2: preparación de los datos para el entrenamiento
Separar el corpus  el conjuntos entrenamiento y prueba . Recordar que el conjunto que prueba debe ser creado de manera aleatoria, por lo tanto, debe de fijarse una semilla para lograr reproducibilidad.
Hacer un análisis exploratorio del conjunto de entrenamiento para decidir sobre el siguiente paso. Una guía es la siguiente: https://neptune.ai/blog/exploratory-data-analysis-natural-language-processing-tools
En función del análisis previo: limpiar, normalizar, segmentar y tokenizar el corpus de entrenamiento.  
Las palabras poco frecuentes transformarlas en el token <UNK>. 
Una vez armado el corpus de entrenamiento, construir el corpus ordenado, listo para ser usado en el modelo de n-gramas, debe tener la estructura [['token','token', ...'token'],['token','token', ...'token'] .. ['token','token', ...'token']]. 
Crea el vocabulario
LIBRETA 3:  

A. Entrenamiento de modelos

Considerar los siguientes modelos para entrenarlos en sintonía con https://www.nltk.org/api/nltk.lm.html.
Modelo 1: unigramas
Modelo 2: bigramas
Modelo 3: suavizado de Laplace
Modelo 4: escoger un suavizado de la librería
B. Evaluación intrínseca de modelos
Al conjunto de prueba aplícale exactamente el paso 3 de la libreta 2. 
A las palabras fuera del vocabulario cámbialas por el token <UNK>
Calcula la perplejidad de cada uno de los modelos
C. Generación del texto

Con cada uno de los modelos entrenados, haz programa que te genere  automáticamente frases de AMLO. 

D. Conclusiones finales
