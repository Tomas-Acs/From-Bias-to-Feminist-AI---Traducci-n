# Capítulo 3: Eliminación del sesgo del algoritmo

Este capítulo explora la ética, las definiciones y las métricas de las conversaciones sobre la equidad, y explora cómo incluso cuando los modelos los tienen en cuenta, la forma en que se implementan y utilizan en el mundo real es igualmente importante.

Escrito por *Elisa Celis*
Publicado en 13 de septiembre de 2021.

---

A menudo existe la percepción de que los sistemas de inteligencia artificial (IA) son matemáticos, compuestos de lógica y maquinaria, y, por lo tanto, imparciales y separados de cuestiones morales. Sin embargo, no existe sólo un conjunto de cosas que signifiquen "IA" y otro conjunto de cosas que signifique "humano". Los dos están fundamentalmente entrelazados debido a la naturaleza de cómo construimos y usamos los sistemas de IA.

En primer lugar, debemos comprender que los datos utilizados en muchos sistemas de IA recopilan simplemente una captura breve de una parte del comportamiento humano. Y como se señaló en [Intro to "Raw Data" is an Oxymoron], la persona que sostiene la cámara decide qué foto tomar y a quién tomarla. Qué datos se usan y recopilan, cómo se limpian y procesan, qué decidimos optimizar y qué métricas usamos para medir el éxito: cada una de estas es una decisión humana informada igualmente por nuestro conocimiento computacional y nuestra intuición humana.

Además, debemos comprender el impacto de la IA en la sociedad. Actualmente, las personas, los gobiernos y las organizaciones consumen productos de IA de manera que afectan fundamentalmente la información a la que tenemos acceso y, por lo tanto, influyen directamente en las oportunidades que tenemos y las decisiones que tomamos. Un sistema que proporciona principalmente opciones de empleo bien remunerado a los hombres que buscan trabajo (Datta et al., 2018), o sugiere posibles opciones de compra de vivienda, principalmente a los blancos que buscan una casa (Sisson, 2019), es uno que perpetúa y exacerba la discriminación ya presente en la sociedad.

![ ](https://raw.githubusercontent.com/sjcr23/From-Bias-to-Feminist-AI-Traduccion/capitulo3/.github/images/Capitulo3/AI%20and%20society%20are%20inseparable.png)

## El panorama de investigación de la eliminación de sesgos en la IA

Estamos en un momento muy emocionante en cuanto a la investigación con respecto a la comprensión de la IA discriminatoria y la búsqueda de métodos algorítmicos para mitigar y eliminar estos sesgos. Si tenemos un problema específico enmarcado en el contexto de la informática, tenemos una amplia variedad de herramientas que pueden ayudarnos a intervenir y controlar la salida para cumplir con una variedad de criterios de equidad y, por lo tanto, reducir la discriminación propagada.

La comunidad informática comenzó a involucrarse en esta área hace menos de 10 años. Al principio, un gran cuello de botella desde una perspectiva algorítmica fue que hay muchas formas de conceptualizar la equidad (Narayanan, 2018). Y no estaba claro cuál, si había alguno, era el adecuado para estudiar. Mirando fuera de nuestro campo, quedó claro que no existe una definición correcta, la idoneidad de cualquier métrica de equidad depende del contexto, los valores y las preferencias de las partes interesadas (Selbst et al., 2019; Verma & Rubin, 2018). Desde una perspectiva algorítmica, esto es muy preocupante, ya que el diseño de algoritmos imparcial aparentemente tendría que resolver un nuevo problema desde cero cada vez que aparece un nuevo contexto. Si bien esto podría hacerse, sería increíblemente ineficiente.

Para abordar esto, junto con fantásticos colegas y estudiantes, recientemente pudimos lograr un gran progreso al pensar que las métricas de equidad pertenecen a una familia de definiciones (Celis et al., 2019). Esto nos permite diseñar marcos de trabajo (frameworks) algorítmicos que funcionan con cualquier definición proveniente de esa familia. Como diseñadores de algoritmos, ya no tenemos que proponer lo que suponemos que podría ser una buena definición de equidad o reinventar la rueda en cada instancia. En cambio, podemos diseñar meta-algoritmos para un caso de uso particular, como publicidad, clasificación o tipos de votación para esta familia de métricas de equidad (Celis et al., 2018; Zafar et al., 2019; Celis et al., 2019). Luego, cuando alguien quiera aplicar un algoritmo sin sesgo a una configuración particular, puede hacer la tarea (ciertamente aún difícil) de desarrollar la definición de equidad correcta y simplemente dársela al marco algorítmico.

![ ](https://raw.githubusercontent.com/sjcr23/From-Bias-to-Feminist-AI-Traduccion/capitulo3/.github/images/Capitulo3/podium.png)

Podemos ilustrar esto con un problema de clasificación (Celis et al., 2018; Celis et al., 2020). Digamos que está contratando y tiene un algoritmo que preseleccionará a sus candidatos y le dará una lista de los 10 mejores candidatos para entrevistar. Ese es un problema de clasificación. Si está contratando en una gran empresa, es posible que tenga diferentes currículos de empleados anteriores y su desempeño y otras métricas. Esos son los datos con los que trabajaremos. Luego, también le pediríamos que defina lo que quiere decir con un resultado justo o imparcial.

Por ejemplo, puede decir que la lista corta debe contener el mismo número de hombres y no hombres. Tal vez eso sea algo razonable para su entorno, o tal vez prefiera que la lista refleje la demografía de los solicitantes según el género y la raza. De cualquier manera, una vez que cuantifique qué atributos protegidos desea tener en cuenta (p. ej., raza o género) y qué métrica de imparcialidad desea utilizar (p. ej., representación equitativa o tasas de error similares), el marco de trabajo de eliminación de sesgo puede tomar eso como entrada para proporcionar una solución personalizada.

![ ](https://raw.githubusercontent.com/sjcr23/From-Bias-to-Feminist-AI-Traduccion/capitulo3/.github/images/Capitulo3/people%20saying%20me.png)

![ ](https://raw.githubusercontent.com/sjcr23/From-Bias-to-Feminist-AI-Traduccion/capitulo3/.github/images/Capitulo3/ads.png)

![ ](https://raw.githubusercontent.com/sjcr23/From-Bias-to-Feminist-AI-Traduccion/capitulo3/.github/images/Capitulo3/hands.png)

**Polarización Anuncios en línea Votación de ganadores múltiples (Celis et al., 2019) (Celis et al., 2019) (Celis et al., 2018)**

![ ](https://raw.githubusercontent.com/sjcr23/From-Bias-to-Feminist-AI-Traduccion/capitulo3/.github/images/Capitulo3/girl%20with%20a%20bunny.png)

![ ](https://raw.githubusercontent.com/sjcr23/From-Bias-to-Feminist-AI-Traduccion/capitulo3/.github/images/Capitulo3/balance.png)

![ ](https://raw.githubusercontent.com/sjcr23/From-Bias-to-Feminist-AI-Traduccion/capitulo3/.github/images/Capitulo3/podium%20with%20childs.png)

![ ](https://raw.githubusercontent.com/sjcr23/From-Bias-to-Feminist-AI-Traduccion/capitulo3/.github/images/Capitulo3/more%20people.png)

**Clasificación Reequilibrio Ranking Muestreo**

(Celis et al., 2019) (Celis et al., 2020) (Celis et al., 2018; (Celis et al., 2017;Celis et al., 2020) Celis et al., 2018)

Ciertamente no hemos terminado, pero esta perspectiva del marco de trabajo es realmente crucial porque ya no tenemos que reinventar la rueda. La excusa "nos gustaría poder implementar algo que no discrimine, pero no tenemos los recursos para desarrollarlo" ya no es válida, ya no tienes que empezar de cero. Junto con mis colegas, ahora tenemos un conjunto de tales marcos de desarrollo para resolver muchos de los grandes problemas en IA uno de estos algoritmos (Controlling Bias in Artificial Intelligence, 2021), y hay varios otros conjuntos de herramientas disponibles para uso de los profesionales (Bellamy et al. al., 2018; Bird et al., 2020).

![ ](https://raw.githubusercontent.com/sjcr23/From-Bias-to-Feminist-AI-Traduccion/capitulo3/.github/images/Capitulo3/fair%20ia%20as%20part%20of%20a%20system.png)

## Grandes desafíos por delante

**Si bien hay muchas razones para ser optimistas, también quedan muchos desafíos importantes por delante en este campo. Estas preguntas profundas se pueden clasificar aproximadamente de la siguiente manera: las técnicas (que se encuentran principalmente en el dominio de la informática), las humanas (que se encuentran principalmente en el dominio de la psicología y la sociología) y las civiles (que se encuentran principalmente en el ámbito legal, social y el dominio de políticas). Aquí, describo algunas de las grandes preguntas a considerar y trabajar en colaboración para abordarlas.**

## El sistema tecnológico

### Riqueza de los conceptos de equidad

**Si bien una vez que se han determinado los atributos protegidos y las métricas de equidad, podemos aplicar técnicas algorítmicas de eliminación de sesgos, quedan muchas preguntas importantes.** Por ejemplo: "¿Qué quiero decir con un algoritmo que no discrimina?", "¿Qué espero lograr?" y "¿A quién estoy tratando de servir?". En particular, actualmente corremos el riesgo de definir la eliminación de sesgo de manera demasiado estrecha. Esta pregunta es en parte filosófica pero también técnica; por ejemplo, comprender que la discriminación ocurre de manera interseccional, ¿Qué técnicas algorítmicas pueden extenderse de manera eficiente a medidas interseccionales de equidad?

Un cuello de botella importante es que, probablemente, en la mayoría de las situaciones no se puede satisfacer más de una definición de equidad simultáneamente (Chouldechova, 2017; Pleiss et al., 2017). Por lo tanto, necesitamos desarrollar una mejor teoría para este problema de equidad multiobjetivo en el que probablemente tendríamos que reenfocar nuestro objetivo para encontrar soluciones que no sean "demasiado" injustas para ninguna métrica (Reich & Vijaykumar, 2021); esta es todavía un área incipiente pero importante para desarrollar.

### Atributos protegidos

Una gran pregunta que recientemente comenzamos a abordar es "¿Qué pasa si no conocemos los atributos protegidos en los datos"? Por ejemplo, en el contexto de EE. UU., es ilegal recopilar información demográfica para usarla como parte de un proceso de contratación. Esto tiene sentido en el sentido de que uno quiere proteger a los grupos de personas que pueden sufrir discriminación, pero también limita las intervenciones directas que puede aplicar si desea reducir los sesgos implícitos (Taslitz, 2007; Bonilla-Silva, 2013). La falacia central de un enfoque de ceguera es que incluso si la categoría no se captura explícitamente en los datos, está implícitamente codificada en las otras características, ya que no se puede separar la demografía de una persona de su experiencia vivida (Apfelbaum et al., 2010). En líneas de trabajo muy recientes hemos comenzado a abordar esta cuestión con nuevas técnicas algorítmicas de eliminación de sesgo que pueden trabajar implícitamente sobre los datos sin atributos protegidos (Celis & Keswani, 2020; Keswani & Celis, 2021), y/o pueden funcionar incluso si el los atributos protegidos tienen errores (Mehrotra & Celis, 2021; Celis et al., 2021).

### Errores de composición

Una idea errónea común es que hay una sola "IA" que controla las decisiones; en realidad, a menudo es un mosaico de algoritmos y componentes que juntos construyen un sistema completo con muchos puntos de decisión en el camino. En esencia, un montón de algoritmos diferentes que funcionan juntos. Donde puede haber una parte en la que el sesgo o la discriminación se infiltran de manera más evidente, los otros componentes no pueden ignorarse, ya que desempeñan un papel en la preparación del resto para el éxito o el fracaso.

Un ejemplo en el que esto ciertamente sucede es la búsqueda web (Google, 2020). Cuando comienzas a buscar algo, Google no va y busca en todo Internet en ese momento; eso simplemente no sería lo suficientemente rápido. Ya se ha realizado una gran cantidad de preprocesamiento en la web, además es probable que se realice una clasificación de relevancia "rápida y sucia" para que pueda funcionar con un subconjunto mucho más pequeño de resultados potenciales. Luego puede explorar este subconjunto mucho más pequeño con más detalle y producir una clasificación de los resultados. Cuando pensamos en la equidad, a menudo consideramos este último paso del proceso: "¿Cómo me aseguro de que mi clasificación sea relevante y justa?" Si bien este es, por supuesto, un componente crucial del problema, si solo le diera al algoritmo de clasificación una muestra muy sesgada para trabajar, la clasificación estaría funcionando con una mano atada a la espalda.

Considere la contratación, un lugar en el que la toma de decisiones algorítmica se ha demostrado repetidamente que es discriminatorio (Ajunwa, 2019; Hamilton, 2018). Si en el proceso de preselección eliminé a muchas candidatas, en el momento en que clasifico mi lista de preseleccionados simplemente no tengo suficiente con qué trabajar. El problema es doble: es posible que simplemente no tenga suficientes mujeres para considerar, y las que tengo pueden no ser tan directamente relevantes para mi tarea. Es tan importante abordar la primera parte del proceso como la clasificación final si queremos producir un grupo diverso de candidatos de calidad. De hecho, si solo corrige un componente sin considerar todo el sistema, puede terminar reduciendo la equidad en su sistema (Dwork & Ilvento, 2019).

### Consideraciones éticas adicionales

Garantizar que los sistemas de IA no sean discriminatorios es muy importante. Sin embargo, no es la única consideración ética que debemos tener al diseñar tecnología.

Una consideración importante es la interpretabilidad: la capacidad de comunicar qué y cómo funciona un sistema de IA al público para que un ciudadano promedio pueda entender y confiar en sus predicciones (Rudin, 2019). Este es un paso incluso más allá de las interpretaciones tradicionales de explicabilidad donde el objetivo es que un experto en IA pueda comprender el efecto del sistema (Ribeiro et al., 2016).

Otra consideración es la privacidad. Un gran avance tecnológico fue la introducción de la privacidad diferencial (Dwork, 2008): ahora hay algoritmos ricos con fuertes protecciones de privacidad disponibles y en uso por grandes empresas, incluidas Apple y Google (Cormode et al., 2018). Sin embargo, hay muy poco trabajo o exploración en torno a los objetivos combinados (y algo ortogonales) de privacidad y equidad (Suriyakumar et al., 2021).

Una vez que comenzamos a observar una variedad de consideraciones éticas, cómo interactúan con nuestras técnicas actuales y dónde permanecen esas brechas técnicas que nos permiten aprovechar los grandes éxitos en cada área por separado.

## El sistema humano

Todo lo que he hablado hasta ahora se centra en los componentes tecnológicos de la eliminación del sesgo. Esta es una pieza crucial, pero es solo una parte del sistema más amplio en el que se utilizan las herramientas de IA. Como tal, debemos pensar en cómo encaja esta pieza en el contexto más amplio de un sistema tecnológico como un todo. ¿Cómo interactúa la parte tecnológica con las personas que la utilizan? Tenemos que considerar tanto a las personas que usan la tecnología directamente como a las que se verán afectadas indirectamente.

### Punto de vista de las partes interesadas

Una pregunta importante a considerar es ¿cuál es la expectativa de justicia de un laico en un sistema de IA? Si realmente hablas con la gente, ¿qué es lo que quieren? ¿Qué creen que es justo? ¿Y cómo varía esto dependiendo de su nivel socioeconómico, interés y conocimiento sobre tecnología, y potencial para ser impactado directamente? Una cosa es que los investigadores y especialistas en ética conceptualicen qué diferentes nociones de justicia “tienen sentido”, y otra es preguntar directamente a aquellos que se verían afectados. Es importante pensar en lo que la gente realmente quiere. Y quizás lo más importante es que debemos detenernos y comprender a las partes interesadas directas que se ven afectadas, especialmente aquellas que provienen de poblaciones vulnerables cuyas voces rara vez se escuchan. Esto a menudo significa volver a evaluar cualquier "solución" localmente en el contexto específico en el que se va a aplicar, porque cada situación será diferente. Al centrarnos en los más afectados y asegurarnos de que las comunidades participen en el proceso de diseño, podemos salir de nuestra arrogancia colectiva como tecnólogos y comenzar a abordar el núcleo de los problemas.

### Humanos "en el ciclo"

También es crucial darse cuenta de que los sistemas de IA a menudo no toman una decisión final. Una de las áreas algorítmicas en las que existe un profundo impacto social está relacionada con la revisión de la libertad condicional o la predicción de la reincidencia. Los sistemas automatizados ahora se utilizan en los EE. UU. para dar a los reclusos o personas arrestadas una "puntuación de riesgo". Esta retroalimentación de IA se le da a un juez, y el juez toma la decisión. Trabajos recientes comienzan a abordar la pregunta de, ¿cómo interactúan la predicción del sistema de IA y la decisión del juez (Green & Chen, 2019)? Esto es similar a la pregunta de composición mencionada anteriormente, excepto que ahora la composición está entre la IA y los componentes humanos. Sabiendo que tanto los sistemas de IA como los jueces pueden estar sesgados, ¿el sistema combinado mejora o empeora los resultados? Hay algunos casos en los que, dependiendo de cómo presentemos la información, cuando redactamos terminamos con algo aún más sesgado (Dwork & Ilvento, 2019). Toda la tubería debe diseñarse y auditarse con mucho cuidado para garantizar que realmente estamos moviendo la flecha en una dirección positiva.

![ ](https://raw.githubusercontent.com/sjcr23/From-Bias-to-Feminist-AI-Traduccion/capitulo3/.github/images/Capitulo3/black%20hands.png)

## El sistema social

El tercer escenario donde quedan grandes desafíos es cuando consideramos el sistema social como un todo. En esto, la IA es, en muchos sentidos, un componente muy pequeño.

### Regulación

¿Cuáles son nuestros valores como sociedad? ¿Y qué políticas y regulaciones necesitamos para estar a la altura de ellas? ¿Qué podemos regular y de qué manera podemos y debemos regularlo? ¿Cómo podemos hacer que todos, desde las grandes empresas tecnológicas hasta los municipios locales, utilicen la IA de manera responsable? Necesitamos trabajar juntos en todas las disciplinas para encontrar soluciones compuestas que tengan sentido para lo que tenemos la tecnología, o reimaginar **lo que podemos diseñar a la luz de lo que se puede regular.** No se trata solo de obtener la tecnología correcta, se trata de obtenerla justo en el contexto en el que se despliega. Una dificultad clave es simplemente aprender a hablar unos con otros. Necesitamos formuladores de políticas para comprender la tecnología y tecnólogos para comprender las implicaciones políticas. En términos de regulación (Crawford et al., 2021; Bonatti et al., 2021). Por ejemplo, un mandato para la recopilación de ciertos tipos de información. Entonces, incluso si desea prohibir el uso de características protegidas en una predicción de IA, es posible que deseemos recopilar esos datos para realizar una auditoría que evalúe el impacto en la demografía. Obligar esto es una propuesta muy concreta, pero incluso llegar a la conclusión de que necesitamos tales mandatos requiere aportes interdisciplinarios.

### Auditorías en curso

Los sistemas algorítmicos, así como los sistemas sociales, son dinámicos. Y, por lo tanto, no podemos pensar en esto como un sistema que se termina y luego se implementa. Tiene que haber un proceso de auditación activo porque el mundo no es estático. Además, una vez que entendemos que las políticas y las tecnologías afectan el comportamiento y las oportunidades individuales, queda claro que al implementar una tecnología, cambiamos el panorama de los datos. Por lo tanto, no estamos operando en un sistema estático donde se puede “aprender una vez”: el proceso es dinámico y el aprendizaje debe actualizarse y evaluarse constantemente. Para ello, necesitamos reguladores de confianza de terceros, no muy diferentes a los que existen para los bancos, que puedan realizar auditorías periódicas y continuas de las grandes empresas de tecnología o de la tecnología que se utiliza en el sector público.

![ ](https://raw.githubusercontent.com/sjcr23/From-Bias-to-Feminist-AI-Traduccion/capitulo3/.github/images/Capitulo3/far%20ai%20as.png)

### Negarse a participar

Otra pregunta que como tecnólogos tenemos que hacernos es, ¿en qué punto nos negamos a construir un sistema, en lugar de tratar constantemente de mejorar o construir uno justo a partir del sesgado que tenemos? Existe una tensión entre hacer todo lo posible para mejorar un sistema que nunca será completamente imparcial y negarse a participar por principio porque incluso lo mejor posible no es lo suficientemente bueno. En resumen, esta es una pregunta de abolición: ¿en qué punto y para qué entornos tenemos que analizar detenidamente y decir que deberíamos argumentar aquí como tecnólogos que este no es un lugar para la IA en absoluto? En general, tenemos muchas lecciones que podemos aprender de los éxitos o fracasos anteriores en los movimientos de justicia social.

### Conclusión

La IA es una herramienta poderosa con impactos que se extienden por todo el mundo. Los cambios que ha traído para mejorar son inmensos, pero también lo son los desafíos que quedan con respecto a garantizar un acceso imparcial y resultados justos. Me ha alentado la reciente actividad interdisciplinaria para abordar estas preguntas, y desafío a otros a unirse a este esfuerzo mientras trabajamos por un mundo mejor para todos.

### Bibliografía

Ajunwa, I. (2019). La paradoja de la automatización como intervención anti-sesgo. Cardozo L.Rev., 41.

Apfelbaum, E. P., Pauker, K., Sommers, S. R. y Ambady, N. (2010). ¿En la búsqueda ciega de la igualdad racial? Ciencias psicológicas, 21.

Bellamy, R. K., Dey, K., Hind, M., Hoffman, S. C., Houde, S., Kannan, K. y Lohia et al., P. (2018). AI Fairness 360: un conjunto de herramientas extensible para detectar, comprender y mitigar el sesgo algorítmico no deseado.

Bird, S., Dudik, M., Edgar, R., Horn, B., Lutz, R., Milan, V., Sameki, M., Wallach, H. y Walker, K. (2020). Fairlearn: un conjunto de herramientas para evaluar y mejorar la equidad en la IA. Microsoft, Tecnología. Reps.

Bonatti, A., Celis, L. E., Crawford, G. S., Dinielli, D., Heidhues, P., Luca, M., Salz, T., Schnitzer, M., Scott Morton, F. M., Seim, K., Sinkinson, M. y Zhou, J. (2021). Búsqueda más competitiva a través de la regulación. El Proyecto de Regulación Digital, Centro Tobin de Política Económica.

Bonilla-Silva, E. (2013). Racismo sin racistas: racismo daltónico y la persistencia de la desigualdad racial en los Estados Unidos. Rowman y Littlefield.

Celis, L. E., Deshpande, A., Kathuria, T., Straszak, D. y Vishnoi, N. K. (2017). Sobre la complejidad de los procesos de puntos determinantes restringidos. Aproximación, aleatorización y optimización combinatoria. Algoritmos y Técnicas.

Celis, L. E., Huang, L., Keswani, V. y Vishnoi, N. K. (2019). Clasificación con restricciones de equidad: un meta-algoritmo con garantías comprobables. Actas de la conferencia sobre equidad, rendición de cuentas y transparencia.

Celis, L. E., Huang, L., Keswani, V. y Vishnoi, N. K. (2021). Clasificación Justa con Atributos Protegidos Ruidosos: Un Marco con Garantías Probables.

Celis, L. E., Huang, L. y Vishnoi, N. K. (2018). Votación de múltiples ganadores con restricciones de equidad. Actas de la 27ª Conferencia Internacional Conjunta sobre Inteligencia Artificial.

Celis, L. E., Kapoor, S., Salehi, F. y Vishnoi, N. K. (2019). Controlando la polarización en la personalización: un marco algorítmico. Actas de la conferencia sobre equidad, rendición de cuentas y transparencia.

Celis, L. E. y Keswani, V. (2020). Diversidad implícita en el resumen de imágenes. Actas de la ACM sobre interacción humano-computadora 4.CSCW2.

Celis, L. E., Keswani, V., Straszak, D., Deshpande, A., Kathuria, T. y Vishnoi, N. K. (2018). Resumen de datos justo y diverso basado en DPP. Conferencia Internacional sobre Aprendizaje Automático.

Celis, L. E., Keswani, V. y Vishnoi, N. K. (2020). Preprocesamiento de datos para mitigar el sesgo: un enfoque basado en la entropía máxima. Conferencia Internacional sobre Aprendizaje Automático.

Celis, L. E., Mehrotra, A. y Vishnoi, N. K. (2019). Hacia el control de la discriminación en las subastas de anuncios en línea. Conferencia Internacional sobre Aprendizaje Automático.

Celis, L. E., Mehrotra, A. y Vishnoi, N. K. (2020). Intervenciones para la clasificación en presencia de sesgo implícito. Actas de la Conferencia de 2020 sobre equidad, responsabilidad y transparencia.

Celis, L. E., Straszak, D. y Vishnoi, N. K. (2018). Clasificación con restricciones de equidad. Coloquio Internacional sobre Autómatas, Lenguajes y Programación.

Chouldechova, A. (2017). Predicción justa con impacto desigual: un estudio del sesgo en los instrumentos de predicción de reincidencia. Grandes datos, 5(2).

Control de sesgo en inteligencia artificial. (2021). https://control-sesgo.github.io/

Cormode, G., Jha, S., Kulkarni, T., Li, N., Srivastava, D. y Wang, T. (2018). Privacidad a escala: privacidad diferencial local en la práctica. Actas de la Conferencia Internacional sobre Gestión de Datos de 2018.

Crawford, G. S., Crémer, J., Dinielli, D., Fletcher, A., Heidhues, P., Luca, M., Salz, T., Schnitzer, M., Scott Morton, F. M., Seim, K. y Sinkinson, M. (2021). Protección al Consumidor para Mercados en Línea y Grandes Plataformas Digitales.

Datta, A., Datta, A., Makagon, J., Mulligan, D. K. y Tschantz, M. C. (2018). Discriminación en la publicidad online: una investigación multidisciplinar. Conferencia sobre Equidad, Rendición de Cuentas y Transparencia.

Dwork, C. (2008). Privacidad diferencial: una encuesta de resultados. Springer, Berlín, Heidelberg.

Dwork, C. e Ilvento, C. (2019). Equidad bajo composición. Congreso Innovaciones en Informática Teórica.

Google. (2020). Cómo organiza la búsqueda la información. https://www.google.com/search/howsearchworks/crawling-indexing/

Green, B. y Chen, Y. (2019). Interacciones dispares: un análisis de algoritmo en el ciclo de la equidad en las evaluaciones de riesgo. Actas de la Conferencia sobre Equidad, Responsabilidad y Transparencia.

Hamilton, IA (2018). Amazon creó una herramienta de inteligencia artificial para contratar personas, pero tuvo que cerrarla porque discriminaba a las mujeres. https://www.businessinsider.com/amazon-built-ai-to-hire-people-discriminated-against-women-2018-10

Keswani, V. y Celis, L. E. (2021). Diversidad de dialectos en resúmenes de texto en Twitter. Actas de la Conferencia Web.

Mehrotra, A. y Celis, L. E. (2021). Mitigación del sesgo en la selección de conjuntos con atributos protegidos ruidosos. Actas de la Conferencia ACM de 2021 sobre equidad, responsabilidad y transparencia.

Narayanan, A. (2018). Tutorial de traducción: 21 definiciones de equidad y sus políticas. proc. Conf. Fairness Accountability Transp., Nueva York, EE. UU., 2(3). https://www.youtube.com/watch?v=jIXIuYdnyyk

Noble, S. U. (2018). Algoritmos de opresión: cómo los motores de búsqueda refuerzan el racismo. Prensa de la Universidad de Nueva York.

Pleiss, G., Raghavan, M., Wu, F., Kleinberg, J. y Weinberger, K. Q. (2017). Sobre la Equidad y la Calibración. Avances en sistemas de procesamiento de información neuronal, 30.

Reich, CL y Vijaykumar, S. (2021). Una posibilidad en la equidad algorítmica: ¿Se pueden conciliar la calibración y las tasas de error iguales? Simposio sobre Fundamentos de la Computación Responsable.

Ribeiro, M. T., Singh, S. y Guestrin, C. (2016). ¿Por qué debería confiar en ti?" Explicando las predicciones de cualquier clasificador. Actas de la 22ª conferencia internacional ACM SIGKDD sobre descubrimiento de conocimiento y minería de datos.

Rudin, C. (2019). Deje de explicar los modelos de aprendizaje automático de caja negra para decisiones de alto riesgo y utilice modelos interpretables en su lugar. Inteligencia artificial de la naturaleza, 1(5).

Selbst, A. D., boyd, d., Friedler, S. A., Venkatasubramanian, S. y Vertesi, J. (2019). Equidad y Abstracción en Sistemas Sociotécnicos. Actas de la conferencia sobre equidad, rendición de cuentas y transparencia.

Sisson, P. (2019). https://archive.curbed.com/2019/12/17/21026311/mortgage-apartment-housing-algorithm-discrimination. Curvado.

Suriyakumar, V. M., Papernot, N., Goldenberg, A. y Ghassemi, M. (2021). Persiguiendo sus colas largas: predicción diferencialmente privada en entornos de atención médica. Actas de la Conferencia ACM de 2021 sobre equidad, responsabilidad y transparencia.

Taslitz, A. (2007). Vista ciega racial: el absurdo de la justicia penal daltónica. Revista de derecho penal del estado de Ohio.

Verma, S. y Rubin, J. (2018). Explicación de las definiciones de equidad. Taller internacional IEEE/ACM sobre equidad de software (Fairware).

Zafar, M. B., Valera, I., Gomez-Rodriguez, M., & Gummadi, K. P. (2019). Restricciones de equidad: un enfoque flexible para la clasificación justa. Revista de investigación de aprendizaje automático, 20.