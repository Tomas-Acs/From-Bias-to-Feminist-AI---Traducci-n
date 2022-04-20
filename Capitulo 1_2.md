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
