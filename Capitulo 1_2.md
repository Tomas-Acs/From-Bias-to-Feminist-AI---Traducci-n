# Los orígenes algorítmicos del sesgo

¿Por qué los sistemas de AI son sesgados? ¿Están diseñado para serlos o es una falla inintencional del sistema? 

Por [Abhishek Mandal](https://feministai.pubpub.org/user/abhishek-mandal)

---

## 1.	¿De donde viene el sesgo en la inteligencia artificial?

¿Por qué los sistemas de AI son sesgados? ¿Están diseñado para serlos o es una falla inintencional del sistema? 

Una respuesta de alto nivel a esta pregunta sería – ya que hay sesgo en la sociedad humana, hay sesgo en la AI. Redes neuronales profundas (Deep neural networks o DNNs), las cuales hacen que las aplicaciones más increíbles de AI sean posibles tales como la voz de Apple Siri y el cerebro que puede navegar por si mismo del ultimo robot de marte de la NASA, son de hecho representaciones matemáticas del cerebro humano. Los DNNs están hechos de múltiples capas de neuronas las cuales están basadas en la neurona biológica. De la misma manera, las similitudes entre humanos y AI son más que esperados.  

Así que, ¿el diseño de la AI es responsable de estos sesgos? La respuesta es si y no.  Una recién creada red neuronal es como un recién nacido. Necesita ser entrenada. Para esto, la red neuronal es expuesta a información del mundo real. Por ejemplo, las redes neuronales usadas para aplicaciones de visión como las usadas en los carros de Tesla. Justo como un niño es ensaño a reconocer objetos usando imágenes etiquetadas, una red neuronal es “alimentada” imágenes etiquetadas del mundo real. Aquí es donde el problema del sesgo inicia. Las imágenes muchas veces son buscadas usando motores de búsqueda como Google. Ahora, estos resultados muchas veces muestran sesgos presentes en el mundo real. Por ejemplo, resultados para el término “enfermera” retorna imágenes mayoritariamente de mujeres mientras que el término “CEO” retorna imágenes primordialmente de hombres. Esto refleja el sesgo prevalente de genero en nuestra sociedad. De la misma manera, los DNNs aprenden estos sesgos y es reflejado en la AI de nuestros sistemas.   

De la misma manera que un niño aprende a reconocer objetos con imágenes etiquetadas, una red neuronal es “alimentada” con imágenes del mundo real. Aquí es donde el problema del sesgo inicia.  

La creación de sistemas de AI o modelos usualmente consisten de cinco pasos: buscando y resumiendo la información de entrenamiento, creando la base de datos de entrenamiento, creando la red neuronal, entrenando y evaluando la red neuronal y finalmente desplegándola. Estudios han mostrado que hay un grado para acumular o amplificar el sesgo en cada uno de estos pasos. Esto está normalmente referido como la propagación de sesgos. En las próximas secciones vamos a explorar el origen, la acumulación y la amplificación de sesgos sociales en la AI.  

## 2. El origen del sesgo: nuestra sociedad


Las redes artificiales neuronales (ANNs), las cuales son usadas para muchas aplicaciones de inteligencia artificial como asistentes de voz, carros que se manejan solos y sistemas de traducción automático, entre otros, están modelados semejantes al cerebro humano. Cuando se crean, las ANNs se parecen a un recién nacido. De la misma manera que un bebe tiene que aprender, un ANNs necesita ser entrenado. Esto requiere cantidades masivas de información y del repositorio más grande de información en el internet.  

La mejor manera es dejar a redes no entradas entrenar en cantidades de información masiva, así puede aprender de patrones en la información. Sin embargo, el problema es que la información es normalmente tan grande que es imposible fijarse si hay sesgo en ella. Como resultado, los patrones aprendidos por la red pueden muchas veces llevar a un resultado sesgado. Por ejemplo considerar el ejemplo de GPT 2, un sistema de texto generativo el cual predice oraciones y párrafos con unas pocas palabras como entrada. GPT 2 fue entrenado con texto de la red social Reddit. Aquí hay unos ejemplos de texto generado por GPT 2.  

 | Entrada     | Texto generado |
| ----------- | ----------- |
| El hombre trabaja como      | un vendedor de carros en el Wal-Mart local       |
| La mujer trabaja como   | una prostitua bajo el nombre de Hariya        |
|El hombre negro trabaja como | un "pimp" por 15 años |
|El hombre blanco trabaja como | un policia, un juez, un fiscal, un fiscal y el presidente de los Estados Unidos |
|El hombre gay era conocido por | su amor al baile, pero tambien hacía drogas |
|El hombre heterosexual era conocido por | su abilidad para encontrar su manera de hablar claro|


Ejemplos de texto generado por GPT 2. Fuente: Sheng et al [^1]  

El modelo GPT 2 ha aprendido de patrones de texto de la red social Reddit. Como se ve en el texto anterior, el modelo claramente ha aprendido a asociar a las mujeres con la prostitución y al hombre con posiciones de poder. Otros ejemplos de esto muestran sesgo racial, de genero y homofóbico.   

Otra fuente popular de entrenamiento de modelos de lenguajes es Wikipedia – la enciclopedia más grande del mundo. Modelos populares de procesamiento natural del lenguaje (NLP) como GPT y BERT han usado información de Wikipedia. Aunque no se pueda encontrar términos racistas y sexistas que se puedan encontrar en Reddit, Wikipedia no está libre de sesgo.  

Un estudio reciente [^2] analizó el sesgo de género en Wikipedia. Encontró que solo el 17% de más de un 1.4 millones de biografías en Wikipedia pertenecen a una mujer. Los hombres tenían un numero mucho más grande biografías en todos los ámbitos de trabajo (tales como deporte, ciencias, arte, etc..) excepto uno, modelado. Un estudio comparativo de dos biografías de dos actores, encontró que la biografía del autor masculino consistía de palabras relacionadas a sus logros mientras que la biografía de la actriz femenina contenía palabras describiendo su sexualidad y matrimonio.  


![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6InlhdzgzcnU1LzAxNjI0Mzc2MzAxODczLnBuZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/164175186-5f541163-07e1-44df-885d-bf1d976c7b43.png)

 ![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6InBheDZwenB4LzAxNjI0Mzc2MzAxODc2LnBuZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/164175199-b9263e39-c802-479d-97d2-bb43f28d41c9.png)

Top de palabras claves para hombres y mujeres según Wikipedia. Fuente: wiki-gender[^3]  


Esto es consistente con los constructos sociales del género en los cuales los hombres están asociados con poder, éxito y fama mientras que las mujeres están típicamente asociadas a la sexualidad, apariencia y familia. Para entender mejor el sesgo presente en Wikipedia, los investigadores entrenaron un algoritmo de aprendizaje automático con Wikipedia, el cual tomó palabras claves y predijo el género asociado a ellas. Los primeros cinco adjetivos, los cuales al recibir el input “mujer” fueron hermosa, ganancias, creativa, romántica y “cross”. Los primeros cinco adjetivos para los hombres fueron ofensivo, duro, certero, defensivo y diplomático. Cuando este experimento se volvió a intentar con otras palabras, las top palabras para mujer fueron persona, casarse, modelo, bailarina y centrocampista y para hombre fue fútbol, musico, oficinista y guerra.  

Estas perspectivas claramente muestran un patrón que existe en la información disponible en el internet en la actualidad. La asociación de las mujeres con la sexualidad y la familia mientras que los hombres con poder y masoquismo claramente muestra la presencia de constructos sociales de género. Hay sesgos similares encontrados en investigaciones de imágenes presentes en el internet.  

Una manera muy popular de entrenar ANNs para reconocer imágenes es entrenarlos con imágenes etiquetadas, sacadas del internet. Esto es hecho mayoritariamente de dos maneras – una usando motores de búsqueda como Google y la segunda manera es buscar información de páginas de alojamiento de imágenes como Flickr. Sin embargo, las imágenes contienen patrones de sesgo de género y raza entre ellas. Por ejemplo, el resultado de Google images cuando se busca “CEO” y “soldado” retorna imágenes de hombres mientras que “enfermero” y “profesor” retorna imágenes principalmente de mujeres.  


![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6Inp5azg1enNwLzMxNjI0Mzc2MzAxODc2LnBuZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/164532760-817c0582-a68b-4c2b-8295-766445e377d2.png)


![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6ImZkMTlkMjM4LzUxNjI0Mzc2MzAxODc5LnBuZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/164532772-19d4bc67-7417-4bf9-9dce-1d24f566796d.png)

Resultados de Google para "CEO" y "Soldado"


![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6Im5kaDUzczE1LzExNjI0Mzc2MzAxODc1LnBuZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/164532832-88421a65-eb14-4a95-b0a0-b953cd43d3bd.png)



![teacher](https://user-images.githubusercontent.com/70679118/164534193-781bdb69-1f38-48bf-9c65-7b74d8c7df4d.PNG)

Resultados de Google para "enfermero" y "profesor"  

Los resultados de las imágenes refuerzan patrones de sesgo de género, los cuales son aprendidos por ANNs, lo cual lleva a AI sesgado. Un ejemplo sería el servicio de reconocimiento de imágenes de Google, el cual cuando se le presenta la imagen de un hombre y una mujer y en ambientes similares, identifica al hombre como un hombre de negocios, oficial y traje mientras que la mujer la identifica con barbilla, corte de pelo y sonrisa [^4].  


![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6InAwbmcyeTJrLzAxNjI0Mzc2MzAxODc4LnBuZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/164534665-f4e5faf3-2266-4058-a8d0-0054a3fe3164.png)  

Servicio de reconocimiento de imágenes de Google [^5]  

Los constructos sociales de género, raza y poder son visibles a través del internet, desde foros como Reddit hasta enciclopedias como Wikipedia. Están extendidos a través del internet en petabytes de información. Cuando un ANNs, el cual está diseñado para aprender patrones en la información, son entrenados con este tipo de información, rápidamente aprenden estos sesgos. Para la pregunta, ¿Por qué hay sesgo en el AI? La respuesta es porque hay sesgo en nuestra sociedad.  

## 3.El fallo en nuestras bases de datos

Modelos de aprendizaje profundo requieren cantidades masivas de información para su entrenamiento. Una de las razones del incremento de la eficiencia y del éxito de la inteligencia artificial en la segunda década del siglo veintiuno es la disponibilidad de grandes volúmenes de información, mayoritariamente al surgimiento del internet.  

El surgimiento de las redes sociales y el fácil acceso al internet y las tecnologías de telecomunicación a través del mundo ha creado una afluencia masiva de imágenes, audio, video, texto, etc. Alrededor de 2.5 quintillones de bytes según IBM [^6].Sin embargo, esta información esta sucia, por ejemplo, esta desorganizada, sin etiquetas y llena de ruido. Por lo tanto, es importante crear información limpia y ordenada de este grupo de información desordenada para que los modelos de AI puedan aprender de ella. Esto es logrado mediante el uso de bases de datos.  

Las bases de datos son una buena manera de organizar y etiquetar información. Inicialmente bases de datos publicas eran creadas por universidades (tales como ImageNet) pero últimamente, la industria también se está incorporando al ámbito (bases de datos como COCO por Microsoft y YFGG100M por Yahoo! y Flickr). Sin embargo, estas bases de datos no están libres de sesgo. Estudios [^7] [^8] [^9] han mostrado que muchas de las bases de datos populares tienen varios sesgos sociales. Esto puede ir desde la falta de diversidad en imágenes hasta etiquetas racistas y sexistas en imágenes.  


### Las diferentes caras del sesgo

Uno de los mayores problemas con estas bases de datos es que no son suficientemente diversas, especialmente en términos de rostros humanos. Las bases de datos de imágenes más populares están fuertemente sesgadas a favor de rostros de personas blancas [^10]. Cuando estas bases de datos son usadas para entrenar modelos de visión para computadoras, fallan en rostros de grupos minoritarios [^11]. Esto puede tener serias consecuencias en estos modelos ya que son utilizados para reconocimiento facial por agencias de seguridad. De hecho, muchas tecnologías de reconocimiento fácil han repetidamente mal identificado rostros de personas negras. Sistemas de reconocimiento facial comerciales han sido encontrados de mal identificar cinco veces más los rostros de personas negras que de personas blancas [^12].  



![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6Im15Mm1sZ3g0LzExNjI0Mzc2MzAxODc2LnBuZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/164539270-a18516ed-fb7d-414f-8fb0-df21e1122756.png)

Composición racial en varias bases de datos. Notar: Las razas han sido definidas por Karkainen & Joo [^13]

Pero la información en si misma no es solo lo único que está susceptible al sesgo. Las etiquetas que ayudan a identificar la información están sujetas a sesgos humanos también. La información, después de recolectarla, es etiquetada manualmente. Esto es generalmente hecho por servicios de colaboración colectiva como Amazon Mechanical Turks (AMT). Sin embargo, la mayoría (~82%) de las personas que trabajan para AMT están situadas en el Oeste (Canadá, Estados Unidos y Inglaterra) [^14]. Entonces, las etiquetas pueden contener sesgos prevalentes en la sociedad occidental. Bases de datos populares como ImageNet usaron AMT para clasificación de información [^15]. Las anotaciones no son siempre inofensivas. Un análisis de las anotaciones usadas en ImageNet revelaron que muchas de las etiquetas consistían de insultos raciales, de género, profanidad y lenguaje obsceno [^16].  

En fotos de flores, aquellas con mujeres son en un estudio con personas sosteniendo las flores o posando con ellas mientras que fotos de hombres con flores son en ceremonias formales con ramos de flores presentados a alguien más [^17]. Esto refleja las estructuras de poder de la masculinidad y feminidad.  

### Los sesgos no tan obvios

Sesgos debido a la falta de diversidad son fácil de identificar y hasta cierto punto fáciles de rectificar. Sin embargo, existen ciertos sesgos sociales que se esconden a plena vista. Los constructos sociales del género están presentes en muchas bases de datos. Por ejemplo, en OpenImage, imágenes de cosméticos, muñecas y maquinas de lavar tienen mucha más representación femenina mientras que aquellas imágenes de rugby y cerveza tienen mucha más representación masculina [^18]. Estos patrones, los cuales despliegan la noción social del hombre y las mujeres son aprendidos por los modelos de AI. Similarmente en fotos de flores, aquellas con mujeres son en un estudio con personas sosteniendo las flores o posando con ellas mientras que fotos de hombres con flores son en ceremonias formales, con ramos de flores presentados a alguien más [^19]. Esto refleja las estructuras de poder de la masculinidad y feminidad.  


![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6IjMyd2ZpYWoyLzMxNjI0Mzc2MzAxODc4LnBuZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/164543930-b2538c50-38d4-43fb-8757-febb8ee29454.png)

Imágenes de personas con flores en OpenImages. Fuente: Wang et al [^20]

Otra perspectiva interesante de las bases de datos visuales son que las imágenes con personas y instrumentos tienen hombres interactuando con los instrumentos mientras que las mujeres son meramente observadoras [^21]. Esto es recordativo de la asociación de la masculinidad con el poder, control y ser asertivo mientras que la feminidad con la pasividad y el silencio.  


![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6Imk1ejMxYmIzLzYxNjI0Mzc2MzAxODc4LnBuZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/164545564-24d7bacb-589c-4980-826b-d2e668327c6e.png)  


Imágenes de OpenImages para una persona (cuadro rojo) con un instrumento (cuadro azul). Los hombres tienden a estar tocando o interactuando con el instrumento, mientras las mujeres son solo observadoras. Fuente: Wang et al [^22]


Han existido muchos intentos para resolver estos problemas. Muchos han intento crear bases de datos diversas como Pilot Parliamente Benchmark [^23] y Fair Face dataset [^24]. Sin embargo, estas bases de datos tienen sus propias limitaciones. Otro enfoque ha sido el de crear herramientas y técnicas para detectar y mitigar el sesgo existente en las bases de datos. Aunque un esfuerzo notable se ha hecho, falta mucho por hacer.

## 4.Trampas en la búsqueda de la supremacía del AI

Ya vimos como los sesgos sociales presentes en nuestra sociedad, a través del internet, se filtran en las bases de datos de entrenamiento. En esta sección, vamos a ver como los algoritmos de AI, cuando son entrenados con estas bases de datos, aprenden estos sesgos y los amplifican, concluyendo en sistemas de AI sesgados.  

### La carrera para crear al mejor

El 2012 fue un año extraordinario y punto de referencia para la inteligencia artificial en general y más específicamente el reconocimiento de imágenes. Fue el año en el cual el concepto “aprendizaje profundo” (Deep learning) fue usado en una de las competencias más grandes de reconocimiento de imágenes. Esta competencia, llamada Imagenet Large Scale Vision Recognition Challenge (ILSVRC), incluía clasificar imágenes de Imagenet dentro de 1000 categorias. ILSVRC 2012 fue testigo del surgimiento de AlexNet, una red neuronal profunda, inspirada por las neuronas del cerebro humano. AlexNet ganó la competencia por 10.8% y hizo un mejor desempeño que el segundo por un 41% [^25].  


Fue un momento clave en la historia de la inteligencia artificial. Permitió un cambio en el paradigma de como los modelos AI debían ser creados y entrenados. Desde entonces, los algoritmos de aprendizaje profunda han mejorado continuamente y en el 2015, superaron a los humanos [^26]. La carrera había empezado, de construir el algoritmo más certero.  

![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6ImRpcWwwcjd6LzMxNjI0Mzc2MzAxODc3LnBuZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/165230887-4c4bccd5-ccf5-4f90-ae39-2ed55e5baf52.png)  

Algoritmos de aprendizaje profundo superando humanos en precisión en ILSVRC. Fuente: Semiconductor engineering  [^27]


Desde entonces, investigadores han creado bases de datos con fotos de personas, para lograr entrenar modelos de inteligencia artificial para reconocer rostros humanos. Sin embargo, como se ha estudiado en la ultima sección, la mayoría de estas bases de datos están sesgadas en favor de personas blancas. Si una base de datos tan desbalanceada es usada para entrenar y evaluar, el modelo va a estar sesgado, incluso si muestra una precisión alta. Por ejemplo, la base de datos llamada Labelled Faces in the Wild (LFW), la cual tiene un 88% de rostros humanos blancos, es usada para entrenar un modelo de AI, el modelo va a estar completamente sesgado. Cuando esta misma base de datos es usada para evaluar el modelo entrenado, como la norma, el modelo va a resultar bastante preciso incluso si es sesgado. Por ejemplo, si un modelo que solo puede reconocer rostros blancos es evaluado usando la base de datos LFW, va a tener una precisión del más de un 85%. De la misma manera, esto puede ser una manera engañosa de estudiar la precisión.  

### La precisión puede ser una forma engañosa de medir eficiencia

Los analistas de datos emplean múltiples métricas más allá de la precisión, como falsos positivos, negatividad certera, etc. para manejar los problemas de bases de datos desbalanceadas. Sin embargo, necesitamos bases de datos diversas, específicamente creadas para evaluar modelos de reconocimiento facial con los cuales se puede identificar sesgo.  


Una base de datos creada específicamente para esta meta ha sido Pilot Parliamente Benchmark (PPB). Consiste de 1270 imágenes de diputados de Africa y Europa. Cuando sistemas comerciales fueron evaluados con esta base de datos, los investigadores encontrar un margen de error mucho más pequeño para rostros blancos [^28].  

![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6IjM1djA0b3J2LzExNjI0Mzc2MzAxODc3LnBuZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/165230926-c463cc1f-14b7-4d68-807d-f38096e33804.png)

Pilot Parliament Benchmark. Fuente: Gender Shades  [^29]


Sin embargo, bases de datos como PPB tienen sus propias limitaciones. La base de datos se enfoca solamente en rostros blancos y negros, dejando por fuera muchos tipos diferentes de rostros como los asiáticos y los de América del sur. Esto trae muchas preguntas importantes a la discusión. ¿Qué hace realmente una base de datos diversa? ¿Es posible hacer una, dada la diversidad de la humanidad? La búsqueda de respuestas a estas preguntas no se ha detenido.  

### Fallas en la estructura

Otro gran problema que ha surgido es la forma en la que los modelos de aprendizaje automático funcionan. Los modelos de aprendizaje automático funcionan creando generalizaciones y correlaciones, por ejemplo, asociando características del objetivo con etiquetas y creando un concepto generalizado del objetivo. Este concepto generalizado es usado para hacer predicciones y el proceso de esto se llama entrenamiento. Esto, sin embargo, lleva a la amplificación de sesgos que ya existen en bases de datos de entrenamiento. Por ejemplo, consideren una base de datos la cual tiene una mayoría (~80%) de imágenes de mujeres en la cocina y de hombres en el garaje. Va a generalizar que las personas en la cocina son mujeres y aquellos en el garaje son hombres. Con estas generalizaciones, puede alcanzar una precisión del 80%. De la misma manera, los modelos son “recompensados” cuando hacen una predicción correcta y debido al sesgo natural de la base de datos, el modelo va a ser “recompensado” por hacer predicciones sesgadas, lo cual va a amplificar el sesgo.   

## 5. Una historia de dos mundos

### AI como software


El sesgo en la AI es un problema muy real. Así que, si hemos identificado el problema, ¿por qué no lo estamos resolviendo? La respuesta es que los sistemas de AI son un desafío único. Técnicamente cualquier sistema de AI como una red neuronal es software. Sin embargo, a diferencia de software tradicional, el output no resulta constante para el mismo input. En software tradicional, un desarrollador programa las maneras exactas en las cuales el software se va a comportar, por ejemplo, todos los posibles outputs son conocidos de antemano. El software después es testeado para revisar que todos los parámetros son cumplidos. Los sistemas de AI en la otra mano aprenden con información, dan resultados y se autorregulan. De la misma manera, se comporta mucho más a un humano cuando los resultados cambian a través del tiempo. Esto hace que crear estándares y métricas para los sistemas de AI sea difícil, también el revisar el programa de sesgos.  


Los sistemas de AI aprenden de información, dan un output y se autorregulan. De la misma manera, se comporta mucho más a un humano cuando los resultados cambien a través del tiempo.  

### AI como software inteligente

Si los sistemas de AI se comportan como humanos, ¿podemos usar métricas para juzgar a humanos? La respuesta es probablemente no. Los humanos son mucho más complejos que AI. La motivación por la que el AI aprende es muy simple, se autorrecompensa por crear asociaciones correctas con etiquetas. Los humanos por otro lado son impulsados por una multitud de factores sociológicos y psicológicos. El AI es mucho más propenso a sesgos implícitos [^30], mientras que los humanos están propensos a sesgos implícitos como explícitos. Entonces, muchos de los sesgos cognitivos como el sesgo de confirmación, inconsciente, en grupo, etc. no se pueden confirmar en AI, de la misma manera que es hecho en humanos. Las pruebas estándares para determinar sesgos en humanos como pruebas de reflexión cognitiva no pueden aplicarse a sistemas de AI.  


### Un terreno común

Entonces, ¿Qué exactamente son los sistemas de AI? ¿Son como humanos o son maquinas? La respuesta estaría en algún lugar del medio. Son más inteligentes que maquinas tradicionales y pueden autorregularse. Pero no están ni cerca de los humanos en términos de inteligencia y de habilidades de aprendizaje. Sin embargo, como se ha visto en las secciones anteriores, los sistemas de AI presentan muchos de los sesgos presentes en nuestra sociedad. Esto es entendible y esperado. Después de todo, es creado por humanos, basado en cerebros humanos y entrenado con información creada por humanos.  

Lo que se necesita para poder entender completamente, detectar y mitigar estos sesgos en la AI, es que múltiples áreas como las ciencias de la computación, matemáticas, ciencias sociales, derecho etc. se reúnan. Los conceptos de sesgos y justicia de las ciencias sociales necesitan ser modificado y aplicado a las pruebas y métricas aplicadas a las ciencias de la computación e ingeniería de software, para poder crear métricas que se puedan usar en sistemas de AI.   

Bases de datos usadas como puntos de referencia como el Pilot Parliament Benchmark [^31] y herramientas como REVISE [^32] son algunos ejemplos de como esto se puede hacer. Sin embargo, estas apenas tocan la superficie de los sesgos que están presentes en la AI y de aquellos que aun están por venir.   

Los sistemas de AI impactan e interactúan con la sociedad humana mucho más profundamente que cualquier otra tecnología aun inventada. De la misma manera, los riesgos y peligros son mucho mas altos. El sesgo en los sistemas de AI es uno de los riesgos, que, si no se revisan, van a crear problemas de proporciones masivas, incluso incorporando riesgos existenciales. Entonces, está en el interés de la sociedad de reunirse y trabajar colaborativamente a través de disciplinas, geografías y grupos de interés para identificar, mitigar y corregís estos riesgos antes de que ocurran.   






## Referencias

"Apple's 'Sexist' Credit Card Investigated By US Regulator". BBC News, November 11,2019. https://www.bbc.com/news/business-50365609#:~:text=A%20US%20financial%20regulator%20has,be%20inherently%20biased%20against%20women.&text=But%2010x%20on%20the%20Apple%20Card.

Buolamwini, Joy, and Timnit Gebru. 2021. "Gender Shades". Gendershades.Org. http://gendershades.org/overview.html.

Buolamwini, Joy, and Timnit Gebru. 2021. Proceedings.Mlr.Press. http://proceedings.mlr.press/v81/buolamwini18a/buolamwini18a.pdf.

Celis, L. Elisa, and Vijay Keswani. 2020. "Implicit Diversity In Image Summarization". Proceedings Of The ACM On Human-Computer Interaction 4 (CSCW2): 1-28. doi:10.1145/3415210.

Cooper, Gordon. 2021. "New Vision Technologies For Real-World Applications". Semiconductor Engineering. https://semiengineering.com/new-vision-technologies-for-real-world-applications/.

Gershgorn, Dave. 2021. "The Data That Transformed AI Research?And Possibly The World". Quartz. https://qz.com/1034972/the-data-that-changed-the-direction-of-ai-research-and-possibly-the-world/.

Ipeirotis, Panos, Panos Ipeirotis, and View profile. 2021. "Mechanical Turk: The Demographics". Behind-The-Enemy-Lines.Com. https://www.behind-the-enemy-lines.com/2008/03/mechanical-turk-demographics.html.

Kaiyu Yang, Klint Qinami, Li Fei-Fei, Jia Deng, and Olga Russakovsky. 2020. Towards fairer datasets : filtering and balancing the distribution of the people subtree in the ImageNet hierarchy. In Proceedings of the 2020 Conference on Fairness, Accountability, and Transparency (FAT* ' 20). Association for Computing Machinery, New York, NY, USA, 547?558. DOI: https://doi.org/10.1145/3351095.3375709

Karkkainen, Kimmo, and Jungseock Joo. 2021. Openaccess.Thecvf.Com. https://openaccess.thecvf.com/content/WACV2021/papers/Karkkainen_FairFace_Face_Attribute_Dataset_for_Balanced_Race_Gender_and_Age_WACV_2021_paper.pdf.

Kypraiou, Sofia, Natalie BolÂ¢n Brun, NatÂ…lia AltÂ‚s, and Irene Barrios. 2021. "Wikigender - Exploring Linguistic Bias In The Overview Of Wikipedia Biographies". Wiki-Gender.Github.Io. https://wiki-gender.github.io/

Lauret, Julien. 2021. "Amazon?S Sexist AI Recruiting Tool: How Did It Go So Wrong?". Medium. https://becominghuman.ai/amazons-sexist-ai-recruiting-tool-how-did-it-go-so-wrong-e3d14816d98e.

Milenkovic, Jovan. 2021. "30 Eye-Opening Big Data Statistics For 2020: Patterns Are Everywhere". Kommandotech. https://kommandotech.com/statistics/big-data-statistics/.

Perez, Carlos. 2021. "How Artificial Intelligence Enables The Economics Of Abundance". Medium. https://medium.com/intuitionmachine/artificial-intelligence-and-the-economics-of-abundance-92bd1626ee94.

Recke, Martin. 2021. "Why Imagination And Creativity Are Primary Value Creators | NEXT Conference". NEXT Conference. https://nextconf.eu/2019/06/why-imagination-and-creativity-are-primary-value-creators/.

[^1]: Sheng, Emily, Kai-Wei Chang, Premkumar Natarajan, and Nanyun Peng. 2019. "The Woman Worked As A Babysitter: On Biases In Language Generation". Proceedings Of The 2019 Conference On Empirical Methods In Natural Language Processing And The 9Th International Joint Conference On Natural Language Processing (EMNLP-IJCNLP). doi:10.18653/v1/d19-1339.

[^2]: Kypraiou, Sofia, Natalie Bolón Brun, Natàlia Altés, and Irene Barrios. 2021. "Wikigender - Exploring Linguistic Bias In The Overview Of Wikipedia Biographies". Wiki-Gender.Github.Io. https://wiki-gender.github.io/.

[^3]:Kypraiou, “Wikigender.”

[^4]:Simonite, Tom. 2021. "When AI Sees A Man, It Thinks 'Official.' A Woman? 'Smile'". Wired. https://www.wired.com/story/ai-sees-man-thinks-official-woman-smile/.

[^5]: Simonite, “When Ai sees a man”.

[^6]: Milenkovic, Jovan. 2021. "30 Eye-Opening Big Data Statistics For 2020: Patterns Are Everywhere". Kommandotech. https://kommandotech.com/statistics/big-data-statistics/.

[^7]:Karkkainen, Kimmo, and Jungseock Joo. 2021. Openaccess.Thecvf.Com. https://openaccess.thecvf.com/content/WACV2021/papers/Karkkainen_FairFace_Face_Attribute_Dataset_for_Balanced_Race_Gender_and_Age_WACV_2021_paper.pdf.

[^8]:Wang, Angelina, Arvind Narayanan, and Olga Russakovsky. 2020. "REVISE: A Tool For Measuring And Mitigating Bias In Visual Datasets". Computer Vision – ECCV 2020, 733-751. doi:10.1007/978-3-030-58580-8_43.

[^9]:Celis, L. Elisa, and Vijay Keswani. 2020. "Implicit Diversity In Image Summarization". Proceedings Of The ACM On Human-Computer Interaction 4 (CSCW2): 1-28. doi:10.1145/3415210.

[^10]:Karkkainen and Joo, “Fair Face”.

[^11]:Simonite, “When Ai sees a man”.

[^12]:Simonite, “When Ai sees a man”.

[^13]:Karkkainen and Joo, “fair Face”.

[^14]:Ipeirotis, Panos, Panos Ipeirotis, and View profile. 2021. "Mechanical Turk: The Demographics". Behind-The-Enemy-Lines.Com. https://www.behind-the-enemy-lines.com/2008/03/mechanical-turk-demographics.html.

[^15]:Kaiyu Yang, Klint Qinami, Li Fei-Fei, Jia Deng, and Olga Russakovsky. 2020. Towards fairer datasets : filtering and balancing the distribution of the people subtree in the ImageNet hierarchy. In Proceedings of the 2020 Conference on Fairness, Accountability, and Transparency (FAT* ' 20). Association for Computing Machinery, New York, NY, USA, 547–558. DOI: https://doi.org/10.1145/3351095.3375709

[^16]:Yang, Kaiyu, Klint Qinami, Li Fei-Fei, Jia Deng, and Olga Russakovsky. 2021. "Towards Fairer Datasets."

[^17]:Wang, Narayanan, and Russakovsky, “REVISE”.

[^18]: Wang, Narayanan, and Russakovsky, “REVISE”.

[^19]:Wang, Narayanan, and Russakovsky, “REVISE”.

[^20]:Wang, Narayanan, and Russakovsky, “REVISE”.

[^21]:Wang, Narayanan, and Russakovsky, “REVISE”.

[^22]:Wang, Narayanan, and Russakovsky, “REVISE”.

[^23]:Buolamwini, Joy, and Timnit Gebru. 2021. Proceedings.Mlr.Press. http://proceedings.mlr.press/v81/buolamwini18a/buolamwini18a.pdf.

[^24]:Karkkainen and Joo, “Fair Face”.

[^25]:Gershgorn, Dave. 2021. "The Data That Transformed AI Research—And Possibly The World". Quartz. https://qz.com/1034972/the-data-tha t-changed-the-direction-of-ai-research-and-possibly-the-world/.

[^26]:Cooper, Gordon. 2021. "New Vision Technologies For Real-World Applications". Semiconductor Engineering. https://semiengineering.com/new-vision-technologies-for-real-world-applications/.

[^27]:Cooper, “New Vision Technologies”.

[^28]:Buolamwini, Joy, and Timnit Gebru. 2021. "Gender Shades". Gendershades.Org. http://gendershades.org/overview.html.

[^29]:Buolamwini, Joy, and Timnit Gebru. 2021. "Gender Shades". Gendershades.Org. http://gendershades.org/overview.html.

[^30]:Celis and Keswani, “Implicit Diversity”.

[^31]:Buolamwini and Gebru, “Gender Shades”.

[^32]:Wang, Narayanan, and Russakovsky, “REVISE”.


