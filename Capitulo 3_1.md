# ¿Qué es la equidad?

Se han hecho muchos esfuerzos para tratar de "desesgazar" los datos y crear un modelo "justo". Pero, ¿qué es la equidad? ¿Y cómo se puede traducir esto en aprendizaje automático?

Escrito por [*Sofia Kypraiou*](https://feministai.pubpub.org/user/sofia-kypraiou)
Publicado en 13 de septiembre de 2021.

---

La equidad en el aprendizaje automático ha atraído la atención de los investigadores de las comunidades de IA, ingeniería de software y derecho, con un aumento constante de trabajos relacionados en los últimos años. Se han hecho muchos esfuerzos para tratar de "desesgazar" los datos y crear un modelo "justo". Pero, ¿qué es la equidad? ¿Y cómo puede esto traducirse en aprendizaje automático?

## ¿Qué es la equidad?

Para empezar, empecemos por lo que no es. La equidad no es un concepto técnico o estadístico y nunca puede haber una herramienta o un software que pueda "eliminar completamente el sesgo" de los datos o hacer que un modelo sea "justo". La equidad es un concepto ético y por tanto contextual. En el mejor de los casos, podemos seleccionar algún ideal de lo que significa ser "justo" en un contexto específico, y luego avanzar hacia su satisfacción en nuestro contexto particular.

Podemos comenzar por examinar la ciencia y la investigación de datos a través de la lente del poder. Preguntar justo a quién, para quién, por quién y con cuyos intereses y metas están en el centro de los datos, el modelo y el sistema. Las respuestas a estas preguntas son contextuales tanto en la sociedad como en las matemáticas, y son el núcleo de un proceso de diseño básico y ético.

|![ ](https://raw.githubusercontent.com/sjcr23/From-Bias-to-Feminist-AI-Traduccion/capitulo3/.github/images/Capitulo3_1/1.png)|
|-|
|![ ](https://raw.githubusercontent.com/sjcr23/From-Bias-to-Feminist-AI-Traduccion/capitulo3/.github/images/Capitulo3_1/2.png)|
|*Equidad e Igualdad en el Derecho Internacional de los Derechos Humanos. Ilustración de la Sección de Derechos de la Mujer y Género del ACNUDH.*|

Existen diferentes escuelas de pensamiento acerca de la equidad y la toma de decisiones éticas. En la actualidad, existen más de 80 pautas éticas diferentes para la IA. En matemáticas, según el último recuento, hay 21 definiciones matemáticas de equidad. Así como no existe una definición única de equidad o ética, tampoco existen acuerdos claros sobre qué definición aplicar en cada situación individual. Estas definiciones pueden incluso anularse entre sí en lo que se denomina el teorema de la imposibilidad[^1], que establece que no más de una de las tres métricas de equidad (asignaciones de riesgo) de paridad demográfica, paridad predictiva y probabilidades igualadas pueden ser válidas al mismo tiempo para un bien. clasificador calibrado[^2]. Por lo tanto, es necesario realizar compensaciones.

Number of publications related to fairness in ML[^3]

Pero, ¿por qué hay tantas definiciones? ¿Por qué un mismo caso puede ser considerado justo según unas definiciones e injusto según otras?

Para explorar, veamos tres métricas de equidad diferentes, dos para grupos y una para individuos, veamos dónde difieren conceptualmente, dónde funcionan y qué brechas crean.

Usaremos el ejemplo de las solicitudes de empleo entre grupos de candidatos masculinos y femeninos.

## Métricas de Equidad de Grupo

Una forma de ver la equidad es usar métricas de equidad de grupo (o propiedad estadística de grupo), donde "los grupos deben recibir tratamientos o resultados similares", lo que significa que grupos como hombres o mujeres deben recibir tasas de aceptación de trabajo similares.

Dos definiciones populares son la paridad demográfica y las probabilidades igualadas:[^4]

**1. Pariedad demográfica [^5][^6]**

> Esto significa que las tasas de aceptación de los solicitantes de los dos grupos deben ser iguales (por ejemplo, el 50 % de los solicitantes masculinos y el 50 % de las femeninas obtienen el puesto).
>  
> Motivación:


## Referencias

![ ](https://raw.githubusercontent.com/sjcr23/From-Bias-to-Feminist-AI-Traduccion/capitulo3/.github/images/Capitulo3_1/3.png)

[^1]:[Kleinberg, Jon, Sendhil Mullainathan, and Manish Raghavan. ‘Inherent Trade-Offs in the Fair Determination of Risk Scores’. ArXiv:1609.05807 [Cs, Stat], 17 November 2016.](http://arxiv.org/abs/1609.05807.)

[^2]:[If we are thinking in terms of potential differences between outcomes for men and women, this means requiring that a z fraction of men and a z fraction of women assigned a probability z should possess the property in question. - Kleinberg, Jon, et al. ‘Inherent Trade-Offs in the Fair Determination of Risk Scores’. ArXiv:1609.05807 [Cs, Stat], Nov. 2016. arXiv.org.](http://arxiv.org/abs/1609.05807.)

[^3]:[Caton, Simon, and Christian Haas. ‘Fairness in Machine Learning: A Survey’. ArXiv:2010.04053 [Cs, Stat], 4 October 2020.](http://arxiv.org/abs/2010.04053.)

[^4]: Mathematical notation: X (features), A (protected attribute =sex), Y (label)
A = 1 is female, A = 0 male

[^5]:[Zafar, Muhammad Bilal, et al. ‘Fairness Constraints: Mechanisms for Fair Classification’. ArXiv:1507.05259 [Cs, Stat], Mar. 2017. arXiv.org.](http://arxiv.org/abs/1507.05259.)

[^6]: Definition: Classifier C satisfies demographic parity if the outcome to be independent of the protected attribute A. Mathematical formulation: P{Y|A=0} = P{Y|A=1}



