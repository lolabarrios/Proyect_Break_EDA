
ANÁLISIS DE BIOMARCADORES Y PROGRESIÓN EN EL CÁNCER DE TIROIDES:
Este proyecto aplica herramientas de análisis de datos y bioinformática para descifrar los mensajes ocultos en las células y entender cómo progresa el cáncer de tiroides. A través del estudio de perfiles moleculares, buscamos identificar patrones que funcionen como biomarcadores de diagnóstico y progresión para avanzar hacia una medicina de precisión.

RESUMEN DEL PROYECTO: 
El estudio se centra en el Carcinoma Papilar (THCA), la neoplasia endocrina más común, utilizando un dataset que combina datos clínicos y genéticos de pacientes con diversas variantes (Clásica, Folicular y Tall Cell).

METODOLOGÍA Y PREPARACIÓN DE DATOS:
Para garantizar la robustez de los resultados, se aplicó un riguroso proceso de limpieza:
-Normalización: Uso de datos transformados en log_2 para comparar niveles de abundancia de mRNA de forma estadísticamente justa5.
-Filtrado de Ruido: Eliminación de genes con baja expresión media ($<0.5$) y baja variabilidad (percentil 25), reduciendo el set inicial de 19,927 genes a aquellos con información diferencial real.
-Pureza Tumoral: Solo se examinaron muestras con más del 60% de pureza para evitar la "dilución de la señal" causada por células del estroma o inmunes.

HALLAZGOS PRINCIPALES:
Análisis Clínico (Univariante y Bivariante):
-Demografía: Se confirma una mayor prevalencia del cáncer de tiroides en mujeres.
-Agresividad por Histología: La variante Tall Cell es intrínsecamente más agresiva, diagnosticándose mayoritariamente en Estadio III, mientras que la variante Folicular tiende a ser menos propensa a la afectación ganglionar.
-El Factor Edad: Existe una dependencia crítica de la edad en la clasificación clínica. En pacientes jóvenes (<55 años), incluso con alta carga ganglionar, se suele categorizar como Estadio I, mientras que en mayores de 55 la clasificación sigue una estructura más tradicionaL.
Análisis Genómico (Multivariante):
-Firma Genética: Mediante Volcano Plots, se identificaron genes clave sobreexpresados en estadios avanzados.
-Diseminación Ganglionar: El perfil genético asocia sus cambios de expresión de forma más fiable a la presencia de ganglios (N1) que al estadio clínico general.
-Diferencias por Edad: En pacientes mayores de 55 años, la señal genética de agresividad es más compacta y uniforme; en jóvenes, la "maquinaria de invasión" puede encenderse antes de que los ganglios sean físicamente detectables.

CONCLUSIONES:
El análisis identificó una firma de 27 genes cuya activación coordinada podría ejecutar el programa de invasión tumoral. Se concluye que el análisis de expresión génica es más diferenciador cuando se estudia en función de la diseminación ganglionar que del estadiaje clínico tradicional.

FUTURAS LÍNEAS DE INVESTIGACIÓN:
-Enfoque Multiómico: Integrar capas de genómica, epigenómica, proteómica y metabolómica para obtener una visión total de la orquesta molecular.
-Potencia Computacional: Implementar herramientas bioinformáticas avanzadas para mapear la correlación e integración de estos datos a gran escala.




