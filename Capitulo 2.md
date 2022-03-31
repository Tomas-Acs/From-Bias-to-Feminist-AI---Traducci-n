# Capitulo 2: Introducción al Feminismo de Datos

Muchas de las técnicas usadas por sistemas de Inteligencia Artificial, desde estadísticas oficiales, historiales de salud, meta data en línea y satélites,
dependen de “entrenamiento” por medio de grandes cantidades de información.

Escrito por [Catherine D'Ignazio](https://feministai.pubpub.org/user/catherine-dignazio) y [Lauren Klein](https://feministai.pubpub.org/user/lauren-klein).  
Publicado el 12 de septiembre, 2021

***
Vivimos en una época de increíble y constante crecimiento del poder computacional. Cuando las primeras computadoras fueron introducidas al público, en 1977, una computadora de ultima línea, la Apple II, venía con 4KB de RAM, una pantalla que solo podía mostrar 24 líneas de texto (solo en mayúscula), y una interfaz para audio en casete para leer y guardar información.[^1]  
Dejando de lado el pasado, si nos colocamos en el presente, ahora tenemos computadoras en formas de teléfono que caben en nuestros bolsillos y en el caso del IPhone 12 Pro de Apple del 2020, puede mantener 1.5 millones de bits de información más que la primera computadora Apple II. Este ritmo de crecimiento es asombroso, hemos sido testigos de un crecimiento igualmente exponencial en nuestra habilidad para recolectar y guardar información de manera digital. Desgraciadamente, también hemos sido testigos de nuestra habilidad para que nuestra información sea recopilada (figura 1b).
 ![Capture1](https://user-images.githubusercontent.com/70679118/154164910-d22d7105-2d13-4e30-aa6d-f0d3588ddd87.PNG) 
 |:--:|
| ![Capture2](https://user-images.githubusercontent.com/70679118/154193823-7c8dc7e8-7afa-40ec-89a5-da72fed8f7f4.PNG) | 
|Figura 1 (a) Una Apple II último modelo, inaugurada en 1977, contaba con 4KB de RAM, una pantalla que solo podía mostrar 24 líneas de texto y una interfaz de casete para leer y guardar información. Imagen de Wikipedia. (b) Hace varios años, investigadores concluyeron que los transistores estaban alcanzando su máximo en relación al tamaño que se podía alcanzar y que la Ley de Moore no se cumpliría. Sin embargo, el poder computacional de hoy en día es lo que permitió a la Dr. Katie Bouman, una estudiante posdoctoral en el MIT, contribuir a un proyecto que involucra el procesamiento y la composición de aproximadamente cinco petabytes de información capturados por el telescopio Event Horizon para crear la primera imagen en toda la historia de un agujero negro. Después de la publicación de esta foto en abril 2019, en la cual mostraba su alegría como uno de los miembros del equipo, Bouman fue acosada en línea. Cortesía de Tamy Emma Pepín/Twitter.| 


El acto de recolectar y guardar información sobre las personas no es, por supuesto, nada nuevo. Desde los registros de todos aquellos fallecidos, los cuales fueron publicados por agentes de la iglesia a inicios de la época moderna, los conteos de las poblaciones Indígenas en los registros coloniales de las Américas, la recolección de información ha sido utilizada como una técnica para consolidar el conocimiento de aquellas personas que se está estudiando, inherentemente consolidando el poder sobre sus vidas. [^2]
La cercana relación entre la información y el poder es posiblemente más visible durante la época histórica que inicia con los registros de aquellas personas capturadas y puestas en barcos de esclavos, reduciendo todo lo que implica ser un humano a números y nombres. Visible a través de los movimientos eugenésicos de finales del siglo diecinueve y principios del siglo veinte, el cual buscaba el uso de la información para cuantificar y justificar la superioridad de las personas blancas sobre cualquier otra. Actualmente en la proliferación de tecnologías biométricas, las cuales la socióloga Simone Browne ha mostrado, son desproporcionalmente usadas para vigilar a personas negras [^3]. 

Cuando Edward Snowden, antiguo contratista de la Agencia de Seguridad de los Estados Unidos, filtró ciertos documentos a los medios en el 2013, reveló hasta que grado el gobierno federal recolectaba información de forma rutinaria de sus ciudadanos, en muchos casos con el más mínimo respeto por la legalidad o ética [^4].  También a un nivel municipal, los gobiernos locales están empezando a recolectar información en todo ámbito, desde los movimientos del trafico hasta las expresiones faciales, en busca de crear ciudades “inteligentes” [^5]. Esto muchas veces se traduce en reinscribir patrones tradicionales urbanos de poder como la segregación, un monitoreo excesivo de comunidades de color y la racionalización de servicios esenciales para las ciudades [^6]. 

Pero los gobiernos no están solos en estos esfuerzos por recolectar y guardar información; las corporaciones también lo hacen con el propósito de ganar dinero. Las palabras y frases que buscamos en Google, las horas del día en las que somos mas activos en Facebook, la cantidad de objetos que agregamos a nuestro carrito en Amazon, todo esto es guardado como información con la cual las corporaciones hacen ganancias. Desde las acciones mas triviales del día, como esquivar el tráfico, darle me gusta a videos de amigos o incluso salir de nuestras casas son información que se vende como pan caliente. Esto no es porque cualquiera de esas acciones son excepcionalmente interesantes, sino porque estas pequeñas acciones pueden ser combinadas con otras pequeñas acciones para generar recomendaciones y anuncios personalizados, en otras palabras, darnos mas cosas que hacer “likear”, comprar y ver. [^7]

Esta es la economía de la información, muchas veces estas corporaciones son ayudadas por científicos académicos, buscan constantemente cuales comportamientos, en línea o locales, quedan por transformar en información y monetizarlos. Nada está fuera del alcance de la “datificación”, como es normalmente acuñado, ni su historial de búsqueda, los gatos de Catherine o el trasero de Lauren que está usando para sentarse en su silla. Por ejemplo, Shigeomi Koshimizu, un profesor de Ingeniería de Tokio está actualmente diseñando matrices de sensores que guardan información en 360 posiciones diferentes mientras esté implantado en una silla [^8]. El propone que las personas tienen un ID único en sus traseros, algo como las huellas dactilares de los dedos. En el futuro, el sugiere, que nuestros carros van a estar diseñados con el ID de nuestro trasero en lugar de llaves o alarmas para identificar al dueño del carro.

Aunque la “datificación” muchas veces raya con lo absurdo, es un problema muy serio. Decisiones en el ámbito cívico, económico e individuales ya están siendo tomadas y cada vez más por sistemas automatizados que iteran por bases de datos masivas. Por ejemplo, PredPol, una compañía de vigilancia fundada en el 20212 por un antropólogo profesor de la Universidad de California, ha sido contratada por más de una década por la ciudad de Los Ángeles para determinar cuales barrios y zonas necesitan mas vigilancia de parte de policías y cuales ignorar. Pero como PredPol está basado en información histórica y las actividades de vigilancia de los Estados Unidos siempre han estado desproporcionalmente vigilando barrios y zonas de color, las predicciones de donde va a ocurrir los crímenes en el futuro se parecen mucho a las actividades racistas del pasado [^9]. Estos sistemas crean lo que la matemática y escritora Cathy O’Neil, en *Weapons of Math Destruction: How Big Data Increases Inequality and Threatens Democracy*, llama un ciclo destructivo de retroalimentación, amplificando los efectos del racismo y la criminalización de la pobreza que ya están presente en los Estados Unidos de América.

La solución de O’Neil es abrir los sistemas computacionales que producen estos resultados racistas. La única manera de comprender porque estos resultados se están generando, es estudiando los propios sistemas. La transparencia es una pieza clave en el proceso para mitigar los efectos de la información sesgada. Aun así, podemos hacer mucho más que estudiar sistemas discriminatorios. Nuestro mundo actual requiere mucho más y aquí es donde la información feminista entra en juego.
La información feminista es una forma de pensar acerca la información, su análisis y su método de representarlo, el cual es fuertemente informado por la rica historia del activismo feminista y la critica feminista. Este tipo de información inicia con la creencia de una equidad entre géneros y reconociendo que este objetivo requiere (para todas las etnias, orientaciones sexuales y ubicaciones en el mundo) un compromiso para examinar la raíz causante de las desigualdades que sufren ciertos grupos en la actualidad. En el caso de PredPol, la información feminista nos requeriría adicionalmente que investiguemos y rastreemos la información sesgada hasta su origen. La raíz causante del racismo sesgado en “los tres puntos informativos más objetivos” que PredPol utiliza es la larga historia de criminalización de los negros en Estados Unidos de América, lo cual produce practicas sesgadas contra ellos, y en consecuencia se produce información histórica, la cual después es usada para desarrollar modelos de riesgo para el futuro [^10]. Rastrear estos lazos de fuerzas históricas y actuales de opresión, nos pueden ayudar a responder la pregunta ética de si este sistema debería existir en lo absoluto [^11]. Este es el trabajo de una información feminista también. En el caso de PredPol, la respuesta en un rotundo no.

Entender esta larga y complicada reacción en cadena es lo que ha motivado a Yeshimabeit Milner, en conjunto con otros activistas de Estados Unidos, matemáticos y organizadores a fundar la Información para las Vidas Negras, una organización dedicada a “usar la Ciencia de datos para crear cambio concreto y medible para cambiar la vida de las comunidades negras” [^12]. Grupos como “Stop LAPD Spying” están usando explícitamente métodos feministas y antirracistas para cuantificar y retar la recolección de información invasiva de parte de los gobiernos [^13]. Periodistas están utilizando la Ingeniería Inversa en algoritmos y recolectando información cualitativa sobre daño maternal [^14]. Artistas están invitando a participantes a crear mapas ecológicos y usar la inteligencia artificial para crear memorias intergeneracionales de familias (figura 2a) [^15]. 

Este tipo de trabajo no está para nada limitado al Norte. En Tanzania, por ejemplo, el grupo DataZetu (“nuestra información” en swahili) ha trabajo con comunidades para organizar una competencia de diseño, la cual tenía como objetivo crear telas con estadísticas de violencia de genero en los patrones, después hicieron una pasarela con los ganadores (figura 2b). Activistas en América latina están documentando, las mujeres, niñas y personas trans asesinadas en femicidios y grupos sociales están creando estándares de información y redes para usar esta información para retar y combatir la violencia de genero [^16]. En Argentina, grupos como Economía Feminista están usando información colectiva para crear guías para votos feministas, los cuales distribuyen a través de una pagina llamada Feminindex (figura 2c). La lista continua. 
![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6InVoamEwMTQ3LzQxNjI5ODE2MjkxMzgwLnBuZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/155918409-16763098-3b15-4c92-bf76-094ca1d0c08a.png)
|:--:|
![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6IjN5NWFhaWQzLzAxNjI5ODE2MjkxMzgwLnBuZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/155918412-17309a01-239f-4ba6-9822-0887abc432e4.png)
![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6Ijc0cnVvMXBjLzcxNjI5ODE2MjkxMzgwLnBuZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/155918417-8edf3245-d680-47ca-a16b-d8b9338ba506.png)
|Figura 2 Definimos la Ciencia de Datos exhaustivamente, a continuación, tres ejemplos. (a) “Not the Only One” por Stephanie Dinkins (2017), una escultura que representa una familia negra a través del uso de inteligencia artificial. El AI está entrenado a través de las voces menospreciadas de personas negras en el sector tecnológico. (b) El desfile de modas – creador por DataZetu, Tanzania Bora Initiative y Faru Arts and Sports Development Organization (2018) – muestra telas llamadas “khanga” que incorporan estadísticas sobre violencia de genero en sus patrones. Este desfile fue el resultado de un concurso y varios talleres. (c) Un pantallazo del proyecto Feminindex, el cual proporciona guías para votantes feministas en Argentina. El proyecto coloca en una tabla de rangos a los políticos basados en sus opiniones en temas feministas, derechos LGBTQ+, aborto y representación igualitaria. También incluye cartas digitales para intercambiar las cuales han sido muy exitosas en redes sociales.| 


Todos estos proyectos son de las Ciencias de Datos. Muchas personas creen que la información son solo números, pero estos proyectos demuestran que la información también consiste en historias y palabras, colores o sonidos o cualquier tipo de información que es recolectada sistemáticamente, organizada y analizada. La *ciencia* de las Ciencias de Datos simplemente implica un compromiso para sistematizar métodos de observación y experimentar. A través de este artículo, deliberadamente dejamos diversos ejemplos de la Ciencia de Datos. Estos vienen desde personas individuales trabajando o grupos pequeños, desde académicos, artísticos, sin intenciones de lucro, periodísticos y de organizaciones con fines de lucro. Esto se debe a nuestra creencia de una definición de la Ciencias de Datos capaz, una que busca incluir en lugar de excluir, una la cual no yergue barreras basadas en credenciales formales, afiliaciones profesionales, el tamaño de la información, complejidad de métodos técnicos o otros factores externos de experiencia. Todos estos factores, han sido usados en el pasado para evitar que las mujeres trabajen en su totalidad en diversas áreas profesionales incluso cuando áreas como la computación, ciencias de datos y muchas otras están construidas sobre información que mujeres proporcionaron y fueron obligadas a aprender por sus propios medios [^17]. Un intento para frenar contra este sesgo histórico es fundamental para la información feminista también. 

## ¿Cuál feminismo? ¿Para quién?

El feminismo se ha definido y usado de muchas maneras. Aquí y en nuestro libro, empleamos el termino feminismo como una taquigrafía para el diverso y amplio grupo de proyectos que luchan contra el sexismo y otras fuerzas de opresión, también como para aquellas que buscan crear un futuro mas justo, equitativo y vivible. Debido al gran tamaño de proyectos que abarca, algunos académicos prefieren utilizar el termino *feminismos*, el cual busca abordar toda la amplitud y a veces incompatibilidades que hay entre las vertientes del activismo feminista y el pensamiento político. Para términos de una lectura fácil, decidimos usar el termino feminismo en este texto, pero nuestro feminismo está intencionado a ser igual de expansivo. Incluye el trabajo de personas regulares e intelectuales, igual que de grupos organizados que han tomado acciones directas para alcanzar una igualdad de género. También incluye el trabajo de académicos y otros críticos culturales, los cuales han usado la escritura para explorar las razones políticas, sociales, históricas y conceptuales detrás de la desigualdad de genero que nos enfrentamos en el presente. 

En este proceso, muchos de estos escritores y activistas han expuesto como el estatus quo de la actualidad es, de muchas maneras, injusto [^18]. Estas injusticias muchas veces son el resultado de la diferencia histórica y contemporánea del poder entre personas, hombres, mujeres y personas no binarias, incluyendo personas cisgénero y transgénero, mujeres blancas y negras, académicos y comunidades indígenas, las personas del hemisferio Norte y el hemisferio Sur. Los feministas analizan esta diferencia de poder para poder cambiarlo. Un enfoque tan grande, uno que incorpora clases sociales, habilidades, etnias y mucho más, puede sonar un poco extraño para aquellos que piensan que el feminismo se trata solo del género, la realidad es que cualquier movimiento por la igualdad de género debe considerar las muchas maneras de privilegio y opresión que se intersecan.

El concepto de *interseccionalidad* es esencial para entender y aplicar información feminista, pongámonos un poco más específicos. El termino fue acuñado por el teorista legal Kimberlé Crenshaw a finales de 1980 [^19]. En la escuela de Derecho, Crenshaw se topó con el caso de antidiscriminación de DeGraffenreid v. General Motors. Emma DeGraffenreid era una mujer negra que buscó trabajo en una fábrica de General Motors en su pueblo. Ella no fue contratada y demandó a GM por discriminación. La fábrica tenía una historia de contratar a personas negras, muchas personas de color trabajaban en puestos industriales y de mantenimiento. También tenían una historia de contratar mujeres, muchas mujeres blancas trabajaban en la fabrica como secretarias. Estos dos puntos claves de evidencia fueron lo necesario para que el juez desestimara el caso, ya que la compañía si contrataba personas negras y mujeres, no podía estar discriminando por raza o género. Pero Creenshaw quería saber sobre discriminación que involucraba raza y género. Esto era diferente para esa época y era real, necesitaba un nombre [^20].

Un punto clave de la interseccionalidad es que no solo describe los puntos que se intersecan de la identidad de cualquier persona (o *posicionalidades* como es a veces acuñado) [^21]. También describe las fuerzas que se intersecan de privilegio y opresión en el trabajo de una sociedad. La *opresión* involucra un maltrato sistemático de ciertos grupos de parte de otros. Ocurre cuando el poder no es distribuido de manera equitativa, cuando un grupo controla las instituciones de leyes, educación y cultura, y lo utiliza para sistemáticamente excluir a otros grupos y darles ventaja a los propios (mantener el estatus quo) [^22]. En el caso de la desigualdad de género, podemos mencionar el sexismo, patriarcado, cissexismo que está presente y es evidente en todo, desde la representación política, la desigualdad salarial y hasta quien habla más alto en una reunión. En el caso de opresión de raza, esto toma forma en racismo y en supremacía blanca. Otras formas de opresión incluyen colonialismo, clasismo y capacitismo. Cada una tiene su historia particular y se manifiesta de forma diferente en cada cultura y contexto, pero todas tienen el factor común que participan grupos dominantes que acumulan poder a costa de otras. Es más, estas fuerzas de poder y privilegio en un lado y la opresión del otro se juntan y multiplican sus efectos. 

Los efectos del privilegio y la opresión no están distribuidos equitativamente a través de todos las personas y grupos, sin embargo. Para algunos, estos se vuelven obvios y una parte de sus vidas cotidianas que no se puede omitir, particularmente para mujeres, personas de color, personas queer y emigrantes, la lista sigue. Si usted es miembro de alguna o de todos estos grupos minoritarios, usted siente los efectos de la opresión y el privilegio en todo momento, desde las decisiones que toma (o no toma) cada día. Estos sistemas de poder son reales como la lluvia. Estas fuerzas de opresión pueden ser difíciles de detectar cuando uno se beneficia de ellas (a esto lo llamamos un *beneficio peligroso* en nuestro libro). Aquí es cuando volvemos a la idea del feminismo de datos. Nuestro punto inicial es algo que el feminismo sabe que es una verdad absoluta, sin embargo, se ignora mucho en el ámbito de las ciencias de datos: el poder no está distribuido equitativamente en el mundo. Aquellos que tienen el poder están desproporcionalmente una elite, heterosexuales, blancos, sin discapacidades, hombres cisgénero del hemisferio norte [^23]. El trabajo del feminismo de datos es primero estudiar como las practicas estándares de la industria de datos sirven para reforzar estas desigualdades existentes y segundo usar la ciencia de datos para retar y cambiar la distribución de poder [^24]. Debajo del feminismo de datos está la creencia y el compromiso para la *co-liberación*: la idea de que sistemas opresivos le causa daños a todos nosotros menosprecia la calidad y validez de nuestro trabajo y nos impide de crear impacto social verdadero y duradero con la ciencia de datos. 

 A través de su propia historia, el feminismo ha estado constantemente trabajo para convencer al mundo que es relevante para todas las personas de cualquier género. Nosotros enfatizamos en el mismo argumento: el feminismo de datos es para todos. (Aquí tomamos prestado una línea de Bell Hooks [^25].) Tal vez ya se nota que los ejemplos que usamos no son solo sobre mujeres, ni son creados por solo mujeres. Esto es porque la información de datos feminista no se trata solo sobre mujeres. Toma más de un genero para tener desigualdad de genero y más de un genero para trabajar hacia la justicia. Hombres, no binarios y personas queer son orgullosos de llamarse a si mismos feministas y usan el feminismo en su trabajo. Es más, el feminismo de datos no se trata solo sobre género. Feministas interseccionales nos han mostrado como la etnia, clase, sexualidad, habilidad, edad, religión, geografía y más factores que en conjunto se afectan el uno con el otro, influyen en las oportunidades y experiencias de cada persona en el mundo.  El feminismo de datos se trata de poder, de quienes lo tienen y quienes no. El feminismo interseccional examina el poder desigual. Y en nuestro mundo contemporáneo, la información es poder también. Ya que la información está guardada de una manera injusta, esto tiene que ser enfrentado y cambiarlo.


# Información feminista en acción
La información es un arma de doble filo. En un sentido muy literal, la información se ha usado como un arma de parte de aquellos que están en el poder para poder consolidarse aún más en él. En efecto, un punto central del feminismo de datos es mostrar como los gobiernos y empresas han usado la información y estadísticas para preservar un estatus quo desigual. Trabajar con información desde un punto feminista requiere saber y reconocer esta parte de la historia. Sin embargo, el reconocer esta parte de la historia no significa que se va a ceder control del futuro a estos poderes del pasado. La información es parte del problema, no hay duda de eso. Pero es parte de la solución. Otro punto central del proyecto de la información feminista es mostrar como el poder de la información se puede controlar.

Para guiarnos en este trabajo, hemos desarrollado siete principios claves. Individualmente y en conjunto, estos principios surgen de la fundación interseccional del pensamiento feminista. Cada capítulo en nuestro libro esta estructurado alrededor de cada uno de los principios. Los siete principios de la información de datos feminista son los siguientes:

![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6IjkyMmpncWM5LzcxNjI5ODE2MjkxMzgwLmpwZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/156299238-124c61f0-2d2f-43b5-bd3b-34da155a629e.jpg)

![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6ImplMWFndXplLzExNjI5ODE2MjkxMzgwLmpwZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/156299246-b4d37679-ffce-4429-b8c9-cd7274e0c1dc.jpg)

Examine power. Data feminism begins by analyzing how power operates in the world.

Examinar el poder. El feminismo de datos empieza por analizar cómo opera el poder en el mundo.
![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6InA1eHV2NDgwLzUxNjI5ODE2MjkxMzgwLmpwZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/156299275-e94d488c-ed2e-4dc4-85c0-c095f65e7eb7.jpg)

![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6Im84ZTh5dGZmLzQxNjI5ODE2MjkxMzgwLmpwZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/156299282-410228d0-9658-41c4-978c-7689a0e8dd8c.jpg)

Challenge power. Data feminism commits to challenging unequal power structures and working toward justice.  

Desafiar el poder. El feminismo de datos se compromete a desafiar las estructuras de poder desiguales y a trabajar por la justicia.

![elevate](https://user-images.githubusercontent.com/70679118/159993619-12433bbe-6ffb-4aa8-bd01-ceadad51399c.PNG)

![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6InprZjJjNG1tLzcxNjI5ODE2MjkxMzY5LmpwZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/156299578-de7d254c-2f59-40ec-867b-f1ebdc2391c4.jpg)

Elevate emotion and embodiment. Data feminism teaches us to value multiple forms of knowledge, including the knowledge that comes from people as living, feeling bodies in the world.  

Elevar la emoción y la corporalidad. El feminismo de datos nos enseña a valorar múltiples formas de conocimiento, incluyendo los conocimientos de las personas en su carácter de cuerpos vivos y sensibles en el mundo.

![rethink](https://user-images.githubusercontent.com/70679118/159993641-9fcd18c0-9386-493b-bded-65c2e62ac541.PNG)

![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6InRwaWZqYTFqLzMxNjI5ODE2MjkxMzc4LmpwZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/156299651-47e0bc2b-6de3-40ef-92c1-346c0a5496b2.jpg)

Rethink binaries and hierarchies. Data feminism requires us to challenge the gender binary, along with other systems of counting and classification that perpetuate oppression.

Repensar los binarismos y las jerarquías. El feminismo de datos nos obliga a desafiar el binarismo de género, así como otros sistemas de cuantificación y clasificación que perpetúan las opresiones.

![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6ImRsczNvdWFkLzYxNjI5ODE2MjkxMzc4LmpwZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/156299687-ebdc07d0-acdf-42a2-bc79-5847c6fee66a.jpg)

![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6IjFtZ290MjR5LzExNjI5ODE2MjkxMzc4LmpwZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/156299733-0f4a3a97-61b1-433f-aca0-a21354b50963.jpg)


Embrace pluralism. Data feminism insists that the most complete knowledge comes from synthesizing multiple perspectives, with priority given to local, Indigenous, and experiential ways of knowing.  

Adoptar el pluralismo. El feminismo de datos insiste en que el conocimiento más completo surge de sintetizar múltiples perspectivas, y prioriza los saberes locales, indígenas y basados en la experiencia.

![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6ImNubGdhOXA5LzQxNjI5ODE2MjkxMzc5LmpwZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/156299776-b16b7303-e09b-40b5-a025-5d4c91693178.jpg)

![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6IjU4Z2YxeWtoLzcxNjI5ODE2MjkxMzc5LmpwZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/156299784-1145c4b5-6bee-4500-859e-b0a357f07155.jpg)

Consider context. Data feminism asserts that data are not neutral or objective. They are the products of unequal social relations, and this context is essential for conducting accurate, ethical analysis.

Considerar el contexto. El feminismo de datos afirma que los datos no son ni neutrales ni objetivos. Son producto de relaciones sociales desiguales, y este contexto es esencial para realizar un análisis ético y preciso.

![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6IjV5aWF2aWtqLzQxNjI5ODE2MjkxMzc5LmpwZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/156299812-b996269f-548b-433e-966a-f7983fb7e668.jpg)

![eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6Im5jMnFxemxqLzQxNjI5ODE2MjkxMzc5LmpwZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6ODAwLCJmaXQiOiJpbnNpZGUiLCJ3aXRob3V0RW5sYXJnZW1lbnQiOnRydWV9fX0=](https://user-images.githubusercontent.com/70679118/156299824-d5043d9a-dd3b-46ea-a933-b1104cc56605.jpg)

Make labor visible. The work of data science, like all work in the world, is the work of many hands. Data feminism makes this labor visible so that it can be recognized and valued.

Hacer visible el trabajo. El trabajo de la ciencia de datos, como todo trabajo en el mundo, es el trabajo de muchas manos. El feminismo de datos hace visible esta labor, para que pueda ser reconocida y valorada.

Los gráficos sobre el feminismo de datos por Catherine D'Ignazio, Lauren Klein and Marcia Diaz, 2020. Traducción al español por Helena Suárez Val. Estos gráficos son de acceso abierto y también están disponibles en francés, coreano y portugués. Pueden ser descargados aquí: http://datafeminism.io/blog/book/data-feminism-infographic/  


En nuestro libro, exploramos cada principio a detalle, con ejemplos del área de la ciencia de datos, definidos exhaustivamente para mostrar el principio en acción. A través del camino, introducimos conceptos feministas claves como la matriz de dominación (Patricia Hill Collins), conocimiento situado (Donna Haraway), y trabajo emocional (Arlie Hochschild), así como nuestras propias ideas de como el feminismo se ve en teoría y práctica.  Para este fin, introducimos a los lectores a un amplio grupo de personas en la vanguardia de la ciencia de datos y la justicia. Esto incluye ingenieros, desarrolladores de software, activistas y organizadores de comunidades, periodistas, artistas y académicos. Esta variedad de personas, y la variedad de proyectos que han creado, nos han ayudado a responder la pregunta: ¿Qué hace un proyecto de datos feminista? Como eventualmente se va a aclarar, un proyecto puede ser feminista en el contenido, en el sentido de que desafía el poder por la materia de este; en forma, desde la perspectiva de que desafía el poder mediante el cambio en la forma en la que se recolecta la información y en el proceso, en el sentido de que desafía el poder construyendo información participativa e inclusiva. Todo lo que une este amplio trabajo de la información es la convicción y el compromiso para tomar acción y un deseo de crear un mundo más equitativo y justo.
Nuestra meta es tomar una posición en contra del estatus quo, en contra de un mundo que nos beneficia, dos profesoras blancas cisgénero del hemisferio norte, al coste de otros. Nuestros principios tienen la intención de funcionar como pasos concretos para que los analistas de datos que buscan aprender como el feminismo puede ayudarlos a trabajar hacia un mundo más justo, y para aquellos feministas que buscan aprender como su trabajo se puede incorporar al mundo de la información de datos. También están dirigidos a profesionales en todas las áreas en las cuales decisiones se están tomando en base a información, igual para comunidades que quieran resistir o movilizar la información que los rodea. Están escritos para todos aquellos que buscan entender de una mejor manera los gráficos y estadísticas que se encuentran el día a día en sus vidas, y para todos aquellos que buscan comunicar el significado de estos.
Reiterando nuestra propuesta, es que el feminismo de datos es para todos. Es para personas de todos los géneros. Lo más importante; se trata mucho más que solo el género. El feminismo de datos es sobre poder, sobre quien lo tiene y quien no, y como esas diferencias de poder pueden ser desafiadas y cambiadas usando la información. Lo invitamos a unirse a este camino hacia la justicia y rehacer nuestro mundo empujado por la información. 
# Más sobre el feminismo de datos
*Información Feminista* es un libro de acceso abierto publicado por el MIT Press en el 2020. Se puede leer gratis de forma en línea en la siguiente página: https://data-feminism.mitpress.mit.edu/ o se puede comprar desde su librería local independiente. 
 
# Referencias 

Alexander, Michelle. The New Jim Crow. The New Press, 2012.

Anderson, Margo J. The American Census: A Social History. Yale University Press, 2015.

Benjamin, Ruha. Race After Technology: Abolitionist Tools for the New Jim Code. 1st edition. Medford, MA: Polity, 2019.

Browne, Simone. Dark Matters: On the Surveillance of Blackness. Duke University Press, 2015.

CHM. ‘Home’. CHM. Accessed 23 May 2021. https://computerhistory.org/.

Cooper, Brittney C., Susana M. Morris, and Robin M. Boylorn, eds. The Crunk Feminist Collection. New York: The Feminist Press at CUNY, 2017.

Crenshaw, Kimberle. ‘Demarginalizing the Intersection of Race and Sex: A Black Feminist Critique of Antidiscrimination Doctrine, Feminist Theory and Antiracist Politics’. University of Chicago Legal Forum 1989, no. 1 (7 December 2015). https://chicagounbound.uchicago.edu/uclf/vol1989/iss1/8.

———. ‘Mapping the Margins: Intersectionality, Identity Politics, and Violence against Women of Color’. Stanford Law Review 43, no. 6 (1991): 1241–99. https://doi.org/10.2307/1229039.

Crossman, Ashley. ‘What Sociology Can Teach Us About Oppression’. ThoughtCo. Accessed 23 May 2021. https://www.thoughtco.com/social-oppression-3026593.

D’Ignazio. ‘Catherine D’Ignazio on Instagram: “There’s Truly Nothing More Pleasing than a #MaineCoonCat in a Rainbow Lei”’. Accessed 23 May 2021. https://www.instagram.com/p/BgxGicVhhTW/.

DuVernay, Ava. 13th. Documentary, Crime, History. Forward Movement, Kandoo Films, Netflix, 2016.

Ehrenreich, Barbara. Witches, Midwives, and Nurses: A History of Women Healers. 2nd edition. New York City: The Feminist Press at CUNY, 2010.

Eubanks, Virginia. Automating Inequality: How High-Tech Tools Profile, Police, and Punish the Poor. New York, NY: St. Martin’s Press, 2018.

Fake, Caterina. ‘Should This Exist’. Should This Exist? Accessed 23 May 2021. https://shouldthisexist.com/.

Farrell, Molly. Counting Bodies: Population in Colonial American Writing. Oxford University Press, 2016.

Gallardo, Adriana. ‘How We Collected Nearly 5,000 Stories of Maternal Harm’. ProPublica. Accessed 23 May 2021. https://www.propublica.org/article/how-we-collected-nearly-5-000-stories-of-maternal-harm?token=gKXJz8oaquJjtQQXfWohwVdXFUbpvysX.

Hooks, Bell. Feminism Is for Everybody: Passionate Politics. Pluto Press, 2000.

Hugs, Robot. ‘Having Trouble Explaining Oppression? This Comic Can Do It for You’. Everyday Feminism, 30 January 2017. https://everydayfeminism.com/2017/01/trouble-explaining-oppression/.

Intellectual Genealogies, Intersectionality, and Anna Julia Cooper: Vivian M. May. Feminist Solidarity at the Crossroads. Routledge, 2012. https://doi.org/10.4324/9780203145050-12.

Johnson, Jessica Marie. ‘Markup Bodies: Black [Life] Studies and Slavery [Death] Studies at the Digital Crossroads’. Social Text 36, no. 4 (137) (1 December 2018): 57–79. https://doi.org/10.1215/01642472-7145658.

Koh, Yoree. ‘Forget Fingerprints: Car Seat IDs Driver’s Rear End’. Wall Street Journal, 18 January 2012, sec. Driver’s Seat. https://www.wsj.com/articles/BL-DSB-8296.

Light, Jennifer S. ‘When Computers Were Women’. Technology and Culture 40, no. 3 (1999): 455–83.

Logipix Ltd. ‘Safe and Smart Cities’. Logipix. Accessed 23 May 2021. http://www.logipix.com/index.php/safe-and-smart-cities.

Mattern, Shannon. ‘Mission Control: A History of the Urban Dashboard’. Places Journal, 9 March 2015. https://doi.org/10.22269/150309.

Mattu, Julia Angwin, Jeff Larson,Lauren Kirchner,Surya. ‘Machine Bias’. ProPublica. Accessed 23 May 2021. https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing?token=z-JINiwkIjlB5pxCVLzVjG9Q2IGCjWJS.

Mogel, Lize. ‘Walking the Watershed-The Project’. Accessed 23 May 2021. https://www.walkingthewatershed.com/home/.

Moraga, Cherríe. This Bridge Called My Back, Fourth Edition: Writings by Radical Women of Color. Edited by Gloria Anzaldúa. 4th edition. Albany: State University of New York Press, 2015.

O’Neil, Cathy. Weapons of Math Destruction: How Big Data Increases Inequality and Threatens Democracy. Penguin UK, 2016.

PredPol. ‘About Us’. PredPol (blog). Accessed 23 May 2021. https://www.predpol.com/about/.

———. ‘Predictive Policing Technology’. PredPol (blog). Accessed 23 May 2021. https://www.predpol.com/technology/.

Raley, Rita. ‘Dataveillance and Countervailance’, 2013. https://escholarship.org/uc/item/2b12683k.

Simon, Patrick. ‘Collecting Ethnic Statistics in Europe: A Review’. Ethnic and Racial Studies 35, no. 8 (1 August 2012): 1366–91. https://doi.org/10.1080/01419870.2011.607507.

Spade, Dean, and Rori Rohlfs. ‘Legal Equality, Gay Numbers and the (After?)Math of Eugenics’. S&F Online. Accessed 23 May 2021. http://sfonline.barnard.edu/navigating-neoliberalism-in-the-academy-nonprofits-and-beyond/dean-spade-rori-rohlfs-legal-equality-gay-numbers-and-the-aftermath-of-eugenics/.

Stop LAPD Spying Coalition. ‘To Observe and to Suspect”: A People’s Audit of the Los Angeles Police Department’s Special Order 1’, 19 March 2013. https://stoplapdspying.org/wp-content/uploads/2013/04/PEOPLES-AUDIT-UPDATED-APRIL-2-2013-A.pdf.

The Latin American Initiative for Open Data. ‘( Guía Para Protocolizar Procesos de Identificación de Feminicidios’. ILDA (blog), 1 September 2020. http://idatosabiertos.org/guia-para-protocolizar-procesos-de-identificacion-de-feminicidios/.

Vaz, Kim Marie, and Gary L Lemons. Feminist Solidarity at the Crossroads: Intersectional Women’s Studies for Transracial Alliance. New York: Routledge, 2012.

Wernimont, Jacqueline. Numbered Lives: Life and Death in Quantum Media. MIT Press, 2019.


[^1]: Después de varios años de vender kits de computadora, los cuales tenían que ser ensamblados en casa. En 1977, tres compañías sacaron al mercado computadoras prefabricadas: La Apple II, la Commodore PET y la TRS-80. Para más información en la historia de la computación, ver la página en línea del museo de la computación, https://computerhistory.org/. Para más información en la historia de las mujeres en la computación, ver Jennifer Light, “When Computers Were Women”, *Technology and Culture 40.3 (July 1999): 455-483*, y mas recientemente, Mar Hicks, Programmed Inequality: *How Britain Discarded Women Technologists and Lost Its Edge in Computing (MIT Press, 2017)*.

[^2]: Sobre estadísticas de muertes leer a Jacqueline Wernimont, *Numbered Lives: Life and Death in Quantum Media (Cambridge, MA: MIT Press, 2018)*; sobre conteo colonial, leer a Morry Farrel, *Counting Bodies: Population in Colonial American Writing (Oxford: Oxford University Press, 2016)*; para leer sobre una encuesta sobre como las naciones Europeas han recolectado estadísticas en minorías étnicas, Patrick Simon, , *“Collecting Ethnic Statistics in Europe: A Review,” Ethnic and Racial Studies 35, no. 9 (2012): 1366–1391*; y para un análisis profundo sobre las políticas del censo de Estados Unidos de America, Margo J. Anderson, *The American Census: A Social History (New Haven, CT: Yale University Press, 1988)*.

[^3]: Para una estimación poderosa para aportar a esta historia, leer a Jessica Marie Johnson, *“Markup Bodies: Black [Life] Studies and Slavery [Death] Studies at the Digital Crossroads,”* Social Text 34, no. 4 (2018): 57–79. Para un estudio que se centra en el legado de la eugenesia, leer Dean Spade y Rori Rohlfs, *“Legal Equality, Gay Numbers and the (After?)Math of Eugenics,”* Scholar & Feminist Online 13, no. 2 (Spring 2016). Para un estudio transhistórico de la vigilancia de las personas negras, leer Simone Browne, *Dark Matters: On the Surveillance of Blackness (Durham, NC: Duke University Press, 2015).*

[^4]: Esto fue algo que comunidades organizadas (especialmente aquellas que son lideradas por miembros que fueron objetivos de vigilancia) y académicos han estado diciendo por años. Existe toda un área interdisciplinaria llamada estudios de vigilancia que teoriza y estudia practicas de vigilancia. La socióloga Simone Browne describe esta área en su estudio del 2015, Materia Oscura: “Desde su aparición, los estudios de vigilancia han estado primordialmente preocupados en como y por que las poblaciones son vigiladas, documentadas y gobernadas en fronteras, ciudades, aeropuertos y en espacios públicos y privados, a través de tecnología biométrica, telecomunicaciones, CCTTV, documentos de identidad y más recientemente a través de redes sociales como Twitter y Facebook” (13). Rita Raley y otros académicos caracterizan la vigilancia moderna como “dataveillance”; leer Rita Raley, *“Dataveillance and Countervailance"*, en *“Raw Data” Is an Oxymoron*, ed. Lisa Gitelman (Cambridge, MA: MIT Press, 2013), 121–145.


[^5]: Por ejemplo, Logipix afirma vender cámaras y software que detecta infracciones de tráfico, rostros y “actividad sospechosa”; leer “Safe and Smart Cities,” Logipix, accessed April 3, 2019, http://www.logipix.com/index.php/safe-and-smart-cities.

[^6]: Con respecto a la segregación, leer Ruha Benjamin, *Race after Technology: Abolitionist Tools for the New Jim Code* (New York: Wiley, 2019). Acerca de la sobre vigilancia, leer Cathy O’Neil, *Weapons of Math Destruction* (New York: Broadway Books, 2016). Acerca de servicios sociales, leer Virginia Eubanks, *Automating Inequality: How High-tech Tools Profile, Police, and Punish the Poor* (New York: St. Martin’s Press, 2018). Para una exploración de como “información cívica” recompila la información para el público, leer Shannon Mattern, “Mission Control: A History of the Urban Dashboard,” Places Journal, March 2015, https://placesjournal.org/article/mission-control-a-history-of-the-urban-dashboard/.

[^7]:Para ver evidencia del gato Maine Coon de Catherine llamado n00b, ver https://www.instagram.com/p/BgxGicVhhTW/.

[^8]:Yoree Koh, “Forget Fingerprints: Car Seat IDs Driver’s Rear End,” *Wall Street Journa*l, January 18, 2012, https://blogs.wsj.com/drivers-seat/2012/01/18/forget-fingerprints-car-seat-ids
-drivers-rear-end/.


[^9]:Para más información sobre PredPol, ver https://www.predpol.com/technology/. Sobre la historia racista de la policía, leer Browne, *Dark Matters; Benjamin, Race after Technology; and O’Neil, Weapons of Math Destruction.*

[^10]:“Sobre Nosotros”, PredPol, accedido el 23 de Julio, 2019, https://www.predpol.com/about/. Incluso después de que las ataduras legales de la esclavitud fueron abolidas con la ratificación de la decimotercera enmienda en 1865, la proliferación de códigos “negros” fueron abundantes. Estas leyes fueron permitidas mayoritariamente en el Sur de los Estados Unidos de forma que restringieron a los ciudadanos negros libertad de movimiento, acceso a oportunidades y protección bajo la ley. Algunas de estas leyes fueron desafiadas por el publico y en las cortes, sin embargo, fue un proceso muy difícil desmantelarlas por completo. De hecho, en la mayoría de los estados del Sur, simplemente fueron reemplazadas por regulaciones que usaban lenguaje ambiguo para justificar las mismas conductas violentas racistas. Estas regulaciones fueron reforzadas por la introducción por las leyes de Jim Crow a finales del siglo diecinueve e inicios del siglo veinte, las cuales legalizaron segregación racial a través de los estados del Sur. Algunos académicos como Michelle Alexander en *The New Jim Crow: Mass Incarceration in the Age of Colorblindess* (New York: New Press, 2012), y cineastas como Ava DuVernay en *The 13th* (Kandoo Films, 2016) han demostrado evidencia innegable que esta parte de la historia no se ha acabado y que sigue en nuestros días de formas de encarcelamiento masivo y políticas racistas.  

[^11]:Ahora existe un podcast dedicado totalmente a la pregunta de que si algún tipo de tecnología debería existir o no: ver Catarina Fake, “Should This Exist?”, accedido April 3, 2019, https://shouldthisexist.com/.

[^12]:Para aprender más sobre Data for Black Lives, visitar http://d4bl.org/.

[^13]:Ver el reporte de Stop LAPD Spying Coalition, “To Observe and to Suspect”: A People’s Audit of the Los Angeles Police Department’s Special Order 1, Stop LAPD Spying Coalition, April 2, 2013, https://stoplapdspying.org/wp-content/uploads/2013/04/PEOPLES-AUDIT-UPDATED-APRIL-2-2013-A.pdf.

[^14]:Ver Julia Angwin, Jeff Larson, Surya Mattu, and Lauren Kirchner, “Machine Bias,” ProPublica, May 23, 2016,https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing y Adriana Gallardo, “Lost Mothers: How We Collected Nearly 5,000 Stories of Maternal Harm,” ProPublica,March 20,2018, https://www.propublica.org/article/how-we-collected-nearly-5-000-stories-of-maternal-harm. Se discute algoritmos de riesgo en detalle en el capitulo 2 y mortalidad materna en el capitulo 1 de *Data Feminism.*

[^15]:Ver, por ejemplo, Lize Mogel, Walking the Watershed (2016–present), accessed July 23, 2019, http://www.publicgreen.com/projects/watershed.html y Stephanie Dinkins, Not the Only One (2017), accessed July 23, 2019, https://www.stephaniedinkins.com/ntoo.html.  

[^16]:La Iniciativa Latinoamericana por los Datos Abiertos (ILDA) ha estado trabajando en un formato de información para recopilar la colección de información sobre femicidios en la región, la cual puede ser accedida aquí: https://idatosabiertos.org/guia-para-protocolizar-procesos-de-identificacion-de-feminicidios/

[^17]:  Este fenómeno, aunque nuevo a las ciencias de datos, es desafortunadamente muy viejo. En su ahora libro clásico, *Witches, Midwives, and Nurses: A History of Women Healers*, Barbara Ehrenreich y Deirdre English detallan la historia de la obstetricia en los Estados Unidos de América, en el cual parteras con experiencia real fueron reemplazadas por ridículos hombres llenos de teoría después del surgimiento de la medicina formal. El mismo fenómeno se puede presenciar en las cocinas, mujeres realizando este acto, sin compensación alguna mientras los hombres atienden a escuelas culinarias para volverse chefs de celebridad. Ver Barba Ehrenreich y Deirdre English, *Witches, Midwives, and Nurses: A History of Women Healers* (New York: The Feminist Press, [1973] 2010).

[^18]: La bibliografía en este tema es vasta. Obras claves incluyen Beverly Guy-Sheftall,* Words of Fire* (New York: New Press, 1995) y Cherríe Moraga and Gloria E. Anzaldúa, *This Bridge Called My Back: Writings by Radical Women of Color* (London: Persephone Press, 1981). Para leer una antología reciente en este ámbito ver *The Crunk Feminist Collection*, editada por Brittney C. Cooper, Susana M. Morris, y Robin M. Boylorn (New York: Feminist Press, 2017).

[^19]: Usualmente los académicos citan dos de los primeros ensayos legales de Crenshaw para el Genesis del término: “Demarginalizing the Intersection of Race and Sex: A Black Feminist Critique of Antidiscrimination Doctrine, Feminist Theory, and Antiracist Politics,” University of Chicago Legal Forum 8 (1989): 139–167 y “Mapping the Margins: Intersectionality, Identity Politics, and Violence against Women of Color,” Stanford Law Review 43, no. 6 (1991): 1241–1299.

[^20]: Mientras Crenshaw nombra el concepto, la idea de interseccionalidad tiene una larga historia en el feminismo negro, notablemente el colectivo Combahee River el cual famosamente describió los sistemas de opresión como “interconectados” en “The Combahee River Colelctive Statement”, 1978, Circuitous.org, accessed April 3, 2019, http://circuitous.org/scraps/combahee.html. Los académicos también  han trazado la interseccionalidad como un concepto hasta el siglo diecinueve, trabajo de la académica y activista Anna Julia Cooper, ver Vivian M. May, *“Intellectual Genealogies, Intersectionality*, y Anna Julia Cooper,” en *Feminist Solidarity at the Crossroads: Intersectional Women’s Studies for Transracial Alliance*, editado por Kim Marie Vaz and Gary L. Lemons (New York: Routledge, 2012), 59–71.

[^21]: *Posicionalidad* es un término que describe como individuos llegan a procesos que forman conocimiento desde múltiples posiciones, incluyendo raza, genero, geografía, clase social, habilidades y más. Cada uno de estás posiciones son moldeadas por la cultura y el contexto, y están constantemente intersecando e interactuando. Nosotros, los autores, tenemos una declaración sobre nuestras propias posicionalidades como un apéndice en *Data Feminism*

[^22]: En la popular página educacional Everyday Feminism, el artista de comics Robot Hugs explica como se siente la opresión en nivel individual: “[It is] when prejudice and discrimination is supported and encouraged by the world around you. It is when you are harmed or not helped by government, community or society at large because of your identity.” “Having Trouble Explaining Oppression? This Comic Can Do It for You,” January 30, 2017, https://everydayfeminism.com/2017/01/trouble-explaining-oppression/. Ashley Crossman  ofrece una buena explicación sociológica de la opresión en *“What Is Social Oppression,”* ThoughtCo, January 28, 2019, https://www.thoughtco.com/social-oppression-3026593.

[^23]: Nosotros discutimos estas demografías y la matriz de dominación que crean y sustentan en detalle en el capitulo 1 de *Data Feminism*


[^24]: Notar que lo ultimo es bastante diferente de usar la información para el bien. Exploramos todas estas diferencias en el capitulo 5 de *Data Feminism.*


[^25]: Ver bell hooks, *Feminism is for Everybody: Passionate Politics* (New York: Pluto Press, 2000).


