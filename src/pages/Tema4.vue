<template>
  <div class="curso-main-container pb-3">
    <BannerInterno></BannerInterno>
    <div class="container tarjeta tarjeta--blanca p-4 p-md-5 mb-5">
      <div class="titulo-principal color-acento-contenido">
        <div class="titulo-principal__numero"><span>4</span></div>
        <h1>Introducción a la inteligencia artificial</h1>
      </div>
      <div class="row justify-content-center mb-5">
        <div class="col-lg-9 my-lg-0 my-3">
          <div class="bg15 p-4 h-100 j1">
            <p class="mb-0">
              La inteligencia artificial ha emergido como una de las tecnologías
              más transformadoras del siglo XXI, revolucionando la manera en que
              procesamos información y resolvemos problemas complejos. Este
              capítulo proporciona una visión general de los conceptos
              fundamentales de la IA, sus aplicaciones prácticas y las
              herramientas esenciales para su implementación.
            </p>
          </div>
        </div>
        <div class="col-lg-3 my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/66.png" alt="" />
        </div>
      </div>
      <Separador> </Separador>
      <div id="t_4_1" class="titulo-segundo color-acento-contenido">
        <h2>4.1 Conceptos fundamentales de IA</h2>
      </div>
      <div class="row justify-content-center mb-5">
        <div class="col-lg-7 my-lg-0 my-3">
          <p>
            La inteligencia artificial representa uno de los avances más
            significativos en la historia de la computación, permitiendo a las
            máquinas emular ciertas capacidades cognitivas humanas. En su
            núcleo, la IA busca crear sistemas que puedan aprender de los datos,
            identificar patrones complejos y tomar decisiones con cierto grado
            de autonomía.
          </p>
          <div class="bg6 p-4 j1 mb-4">
            <p class="mb-0">
              Por su parte, el aprendizaje automático (<i
                ><b>machine learning</b></i
              >) es un subconjunto de la IA que se centra en desarrollar
              algoritmos que pueden mejorar automáticamente a través de la
              experiencia. A diferencia de la programación tradicional, donde
              las reglas se establecen explícitamente, en el aprendizaje
              automático los sistemas aprenden estas reglas a partir de los
              datos proporcionados.
            </p>
          </div>
          <p>
            Un concepto fundamental en IA es el de modelo, que bien se puede
            entender como una representación matemática de un proceso del mundo
            real. Los modelos de IA aprenden patrones en los datos de
            entrenamiento y utilizan este conocimiento para hacer predicciones o
            tomar decisiones sobre nuevos datos.
          </p>
        </div>
        <div class="col-lg-5 my-lg-0 my-3 j1">
          <img class="img-a img-t" src="@/assets/curso/temas/67.png" alt="" />
        </div>
      </div>
      <Separador> </Separador>
      <div id="t_4_2" class="titulo-segundo color-acento-contenido">
        <h2>4.2 Aplicaciones y casos de uso</h2>
      </div>
      <div class="row justify-content-center mb-5">
        <div class="col-lg-5 my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/68.png" alt="" />
        </div>
        <div class="col-lg-7 my-lg-0 my-3">
          <div class="bg4 p-4 h-100 j1">
            <p>
              Las aplicaciones de la IA son vastas y continúan expandiéndose a
              medida que la tecnología evoluciona. En el ámbito empresarial, la
              IA se utiliza para optimizar procesos, predecir tendencias de
              mercado y mejorar la experiencia del cliente. Los sistemas de
              recomendación, por ejemplo, utilizan IA para analizar el
              comportamiento de los usuarios y sugerir productos o contenido
              relevante.
            </p>
            <p class="mb-0">
              Para comprender mejor cómo se desarrollan los proyectos de IA en
              la práctica, es útil examinar el flujo de trabajo típico que
              siguen estos proyectos, como se ilustra en la siguiente
              infografía. Este proceso iterativo comienza con la recolección de
              datos de diversas fuentes, seguido de una fase de preparación
              donde los datos se limpian y transforman. Posteriormente, se
              desarrolla la fase de entrenamiento donde los modelos aprenden de
              los datos procesados, y finalmente se llega a la etapa de
              evaluación y despliegue, donde se mide el rendimiento del modelo y
              se implementa en producción.
            </p>
          </div>
        </div>
      </div>
      <div class="row justify-content-center mb-5">
        <div class="col-auto">
          <div class="titulo-sexto color-acento-contenido">
            <h5>Figura 2.</h5>
            <span
              >Flujo de trabajo en proyectos de inteligencia artificial</span
            >
          </div>
          <img
            class="img-a img-t mb-2"
            src="@/assets/curso/temas/69.svg"
            alt="La Figura 2 se denomina «Flujo de trabajo en proyectos de inteligencia artificial » y presenta una secuencia sobre cuatro momentos: recolección de datos, preparación, entrenamiento y, finalmente, evaluación y despliegue."
          />
          <figcaption>Fuente. OIT, 2024.</figcaption>
        </div>
      </div>
      <div class="row justify-content-center mb-5">
        <div class="col-lg-7 my-lg-0 my-3">
          <div class="bg16 p-4 h-100 j1">
            <p>
              Cada etapa de este flujo presenta sus propios desafíos y
              requerimientos específicos. Por ejemplo, en la fase de recolección
              de datos se debe asegurar no solo la cantidad, sino también la
              calidad y representatividad de los datos. La fase de preparación
              suele ser la más intensiva en tiempo y recursos, ya que de ella
              depende en gran medida el éxito del modelo. Durante el
              entrenamiento, la selección del algoritmo adecuado y el ajuste de
              hiperparámetros son medulares, mientras que en la fase de
              evaluación y despliegue, el enfoque está en garantizar que el
              modelo funcione de manera confiable en un entorno de producción.
            </p>
            <p>
              En el campo de la medicina, la IA está revolucionando el
              diagnóstico por imagen, al permitir la detección temprana de
              enfermedades mediante el análisis automatizado de radiografías,
              resonancias magnéticas y otros tipos de imágenes médicas. Los
              sistemas de IA también están ayudando en el descubrimiento de
              nuevos medicamentos, analizando grandes cantidades de datos
              genéticos y moleculares.
            </p>
            <p class="mb-0">
              La industria manufacturera está aprovechando la IA para
              implementar mantenimiento predictivo, donde los algoritmos pueden
              predecir cuándo una máquina necesitará mantenimiento, antes de que
              ocurra una falla. Esto no solo reduce los costos de mantenimiento,
              sino que también minimiza el tiempo de inactividad.
            </p>
          </div>
        </div>
        <div class="col-lg-5 my-lg-0 my-3 j1">
          <img class="img-a img-t" src="@/assets/curso/temas/70.png" alt="" />
        </div>
      </div>
      <Separador> </Separador>
      <div id="t_4_3" class="titulo-segundo color-acento-contenido">
        <h2>4.3 Herramientas básicas para IA</h2>
      </div>
      <div class="row justify-content-center mb-5">
        <div class="col-lg-4 my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/71.png" alt="" />
        </div>
        <div class="col-lg-8 my-lg-0 my-3">
          <p>
            El desarrollo de soluciones de IA requiere un conjunto específico de
            herramientas y tecnologías. Python se ha convertido en el lenguaje
            de programación dominante en este campo, gracias a su simplicidad y
            a la rica ecosistema de bibliotecas especializadas. Entre las
            bibliotecas más importantes encontramos:
          </p>
          <div class="bg6 p-4">
            <ul class="lista-ul fa-ul mb-0">
              <li>
                <i class="fas fa-check-circle color1"></i
                ><span
                  >Scikit-learn para aprendizaje automático tradicional.</span
                >
              </li>
              <li>
                <i class="fas fa-check-circle color1"></i
                ><span>TensorFlow y PyTorch para aprendizaje profundo.</span>
              </li>
              <li>
                <i class="fas fa-check-circle color1"></i
                ><span>Pandas para manipulación y análisis de datos.</span>
              </li>
              <li>
                <i class="fas fa-check-circle color1"></i
                ><span>NumPy para computación numérica.</span>
              </li>
              <li class="mb-0">
                <i class="fas fa-check-circle color1"></i
                ><span class="mb-0"
                  >Matplotlib y Seaborn para visualización de datos.
                </span>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <p>
        La elección de las herramientas adecuadas dependerá de varios factores,
        incluyendo la naturaleza del problema a resolver, el volumen de datos a
        procesar, y los requisitos de rendimiento del sistema. Es importante
        mencionar que las herramientas son solo un medio para un fin: el
        verdadero valor radica en comprender los principios subyacentes y saber
        cuándo y cómo aplicar cada técnica.
      </p>
      <div class="row justify-content-center">
        <div class="col-lg-5 my-lg-0 my-3">
          <div class="bg14 brad p-2 px-3 h-100 j1">
            <p class="mb-0">
              El futuro de la IA promete ser aún más emocionante, con avances en
              áreas como el aprendizaje por refuerzo, la IA explicable y los
              sistemas de IA más eficientes en términos de recursos
              computacionales. Sin embargo, también debemos ser conscientes de
              los desafíos éticos y de privacidad que surgen con el uso cada vez
              más generalizado de la IA.
            </p>
          </div>
        </div>
        <div class="col-lg-3 my-lg-0 my-3 j1">
          <img class="img-a img-t" src="@/assets/curso/temas/72.png" alt="" />
        </div>
        <div class="col-lg-4 my-lg-0 my-3">
          <div class="p-3 h-100 j1">
            <p class="mb-0">
              La implementación exitosa de soluciones de IA requiere no solo
              conocimientos técnicos, sino también una comprensión profunda del
              dominio del problema y consideraciones éticas sólidas. A medida
              que la tecnología continúa evolucionando, la capacidad de
              adaptarse y aprender nuevas herramientas y técnicas será cada vez
              más importante para quienes se desempeñan en este campo.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Tema4',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
