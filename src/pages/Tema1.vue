<template>
  <div class="curso-main-container pb-3">
    <BannerInterno></BannerInterno>
    <div class="container tarjeta tarjeta--blanca p-4 p-md-5 mb-5">
      <div class="titulo-principal color-acento-contenido">
        <div class="titulo-principal__numero"><span>1</span></div>
        <h1>Fundamentos de datos y estructuras</h1>
      </div>
      <div class="bloque-texto-g color-secundario p-3 p-sm-4 p-md-5">
        <div
          class="bloque-texto-g__img"
          :style="{
            'background-image': `url(${require('@/assets/curso/temas/3.png')})`,
          }"
        ></div>
        <div class="bloque-texto-g__texto p-4">
          <p class="mb-0">
            En el contexto actual de la revolución digital, comprender los
            fundamentos de datos y estructuras se ha vuelto esencial para
            cualquier persona que se desempeñe en el campo de la tecnología.
            Este capítulo explora los conceptos básicos que fundamentan el
            trabajo con datos, desde su naturaleza más elemental hasta las
            estructuras complejas que permiten su organización y manipulación
            eficiente.
          </p>
        </div>
      </div>
      <Separador> </Separador>
      <div id="t_1_1" class="titulo-segundo color-acento-contenido">
        <h2>1.1 Conceptos básicos de datos y análisis</h2>
      </div>
      <div class="row justify-content-center align-items-center mb-5">
        <div class="col-lg-9 my-lg-0 my-3">
          <p>
            En el mundo actual, los datos se han convertido en el activo más
            valioso para las organizaciones y la base fundamental para el
            desarrollo de modelos de inteligencia artificial. Pero ¿qué son
            realmente los datos? En su forma más básica, los datos son
            representaciones de hechos, observaciones o mediciones que, por sí
            solos, carecen de contexto o significado. Es a través del análisis y
            la transformación que estos datos en bruto se convierten en
            información valiosa que permite tomar decisiones informadas.
          </p>
          <div class="row justify-content-center align-items-center bg3 p-0">
            <div class="col-lg-5 my-lg-0 my-3 p-0">
              <img class="img-mov" src="@/assets/curso/temas/4.png" alt="" />
            </div>
            <div class="col-lg-7 my-lg-0 my-3">
              <div class="p-4 j1">
                <p>
                  Cuando se analizan los datos en el contexto de la inteligencia
                  artificial, se debe considerar que estos pueden presentarse de
                  diversas formas. Los datos cuantitativos son aquellos que se
                  pueden medir y expresar numéricamente. Ejemplos incluyen la
                  temperatura diaria de una ciudad, el precio de un producto o
                  el número de usuarios que visitan un sitio web. Estos datos
                  permiten realizar cálculos matemáticos y análisis estadísticos
                  precisos.
                </p>
                <p class="mb-0">
                  Por otro lado, los datos cualitativos describen
                  características o cualidades que no pueden medirse
                  numéricamente. Las opiniones de los clientes sobre un
                  servicio, los colores preferidos en un estudio de mercado, o
                  las respuestas a preguntas abiertas en una encuesta son
                  ejemplos de datos cualitativos. Aunque estos datos no son
                  numéricos por naturaleza, son igualmente valiosos y pueden
                  transformarse en información cuantificable mediante técnicas
                  de procesamiento adecuadas.
                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-3 my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/5.png" alt="" />
        </div>
      </div>
      <Separador> </Separador>
      <div id="t_1_2" class="titulo-segundo color-acento-contenido">
        <h2>1.2 Técnicas de modelado de datos</h2>
      </div>
      <div class="row justify-content-center align-items-center mb-5">
        <div class="col-lg-7 my-lg-0 my-3">
          <p>
            El modelado de datos es un proceso fundamental que permite crear una
            representación abstracta de cómo se relacionan y organizan los datos
            en un sistema. Imaginen que están construyendo una casa: antes de
            comenzar la construcción, necesitan planos detallados que muestren
            cómo se conectarán las diferentes habitaciones y qué función
            cumplirá cada espacio. De manera similar, el modelado de datos nos
            proporciona un “plano” de cómo se estructurará y fluirá la
            información en nuestros sistemas.
          </p>
          <p>
            El proceso de modelado comienza con una visión conceptual de alto
            nivel, donde se identifican las principales entidades o conceptos
            sobre los que se necesita almacenar información y cómo se relacionan
            entre sí. Por ejemplo, en un sistema de comercio electrónico, las
            entidades principales podrían ser “Cliente”, “Producto” y “Pedido”.
            Cada una de estas entidades tendrá sus propias características o
            atributos, y establecerá relaciones con otras entidades del sistema.
          </p>
        </div>
        <div class="col-lg-5 my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/15.png" alt="" />
        </div>
      </div>
      <div class="row justify-content-center align-items-center mb-5">
        <div class="col-lg-3 my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/16.png" alt="" />
        </div>
        <div class="col-lg-9 my-lg-0 my-3">
          <div class="bg2 p-4">
            <p class="mb-0">
              A medida que se avanza en el modelado, se llega a un nivel más
              detallado en el que se define cómo se implementarán estas
              estructuras en los sistemas de almacenamiento de datos. En este
              punto, conceptos como la normalización cobran importancia, ya que
              permiten organizar los datos de manera eficiente y eliminar
              redundancias innecesarias.
            </p>
          </div>
        </div>
      </div>
      <Separador> </Separador>
      <div id="t_1_3" class="titulo-segundo color-acento-contenido">
        <h2>1.3 Estructuras de datos fundamentales</h2>
      </div>
      <div class="row justify-content-center mb-5">
        <div class="col-lg-9 my-lg-0 my-3">
          <p>
            Las estructuras de datos son la columna vertebral de cualquier
            sistema de procesamiento de información. Son formas específicas de
            organizar y almacenar datos que nos permiten acceder a ellos y
            modificarlos de manera eficiente. La elección de la estructura de
            datos correcta puede tener un impacto significativo en el
            rendimiento de nuestros algoritmos de inteligencia artificial.
          </p>
          <p>
            Para comprender mejor las diferentes estructuras de datos y sus
            aplicaciones, consideremos la siguiente tabla comparativa:
          </p>
        </div>
        <div class="col-lg-3 my-lg-0 my-3">
          <img
            class="img-a img-t d-lg-block d-none"
            src="@/assets/curso/temas/17.png"
            alt=""
          />
        </div>
      </div>
      <div class="row justify-content-center">
        <div class="col-lg-10">
          <div class="titulo-sexto color-acento-contenido">
            <h5>Tabla 1.</h5>
            <span
              >Principales estructuras de datos, casos de uso y
              limitaciones.</span
            >
          </div>
          <div class="tabla-a color-acento-botones mb-5">
            <table>
              <caption>
                Fuente: OIT, 2024.
              </caption>
              <thead>
                <tr>
                  <th>Estructura</th>
                  <th>Características principales</th>
                  <th>Casos de uso ideales</th>
                  <th>Limitaciones</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td>Arreglos</td>
                  <td>Acceso directo a elementos, tamaño fijo</td>
                  <td>
                    Datos secuenciales, operaciones de búsqueda frecuentes
                  </td>
                  <td>Tamaño inmutable, inserción/eliminación costosa</td>
                </tr>
                <tr>
                  <td>Listas enlazadas</td>
                  <td>Tamaño dinámico, inserción eficiente</td>
                  <td>Datos que cambian frecuentemente</td>
                  <td>Acceso secuencial</td>
                </tr>
                <tr>
                  <td>Árboles</td>
                  <td>Organización jerárquica, búsqueda eficiente</td>
                  <td>Datos jerárquicos, índices</td>
                  <td>Complejidad de implementación</td>
                </tr>
                <tr>
                  <td class="fst-italic">Hash tables</td>
                  <td>Búsqueda rápida por clave</td>
                  <td>Cachés, diccionarios</td>
                  <td>Colisiones, uso de memoria</td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>
      <div class="row justify-content-center mb-5">
        <div class="col-lg-3 my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/18.png" alt="" />
        </div>
        <div class="col-lg-9 my-lg-0 my-3">
          <div class="row justify-content-center align-items-center mb-4">
            <div class="col-auto my-lg-0 my-3">
              <img
                class="img-a img-t"
                src="@/assets/curso/temas/19.svg"
                alt=""
              />
            </div>
            <div class="col my-lg-0 my-3">
              <p class="mb-0">
                Los arreglos, por ejemplo, son una de las estructuras más
                básicas y ampliamente utilizadas. Imaginemos un
                <em>array</em> como una fila de casilleros numerados: cada
                casillero puede contener un dato, y podemos acceder directamente
                a cualquier casillero conociendo su número. Esta estructura es
                ideal cuando conocemos de antemano el tamaño de nuestros datos y
                necesitamos acceder a elementos específicos rápidamente.
              </p>
            </div>
          </div>
          <div class="bg4 p-3">
            <pmb-0
              >Las listas enlazadas, por otro lado, son como una cadena de
              elementos donde cada uno conoce la ubicación del siguiente. Esta
              estructura es más flexible que los arreglos, ya que podemos
              agregar o eliminar elementos fácilmente, pero requiere más tiempo
              para encontrar un elemento específico, ya que debemos recorrer la
              lista desde el principio.
            </pmb-0>
          </div>
        </div>
      </div>
      <p class="mb-5">
        Los árboles y las hash tables son estructuras más complejas que nos
        permiten representar relaciones jerárquicas y conexiones entre datos.
        Estas estructuras son fundamentales en muchos algoritmos de inteligencia
        artificial, especialmente en áreas como el procesamiento del lenguaje
        natural y el análisis de redes sociales.
      </p>
      <div class="row justify-content-center mb-5 pb-3">
        <div class="col-lg-5 my-lg-0 my-3">
          <div class="bg5 brad p-3 h-100 j1">
            <p class="mb-0">
              La elección de la estructura de datos adecuada dependerá de varios
              factores, incluyendo el tipo de operaciones que necesitamos
              realizar con mayor frecuencia, el volumen de datos que
              manejaremos, y los requisitos de rendimiento de nuestra
              aplicación. Es importante recordar que no existe una estructura
              "perfecta" que sirva para todos los casos: cada una tiene sus
              propias ventajas y desventajas que debemos considerar
              cuidadosamente.
            </p>
          </div>
        </div>
        <div class="col-lg-3 my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/20.png" alt="" />
        </div>
        <div class="col-lg-4 my-lg-0 my-3">
          <div class="bg6 brad p-2 px-3 h-100 j1">
            <p class="mb-0">
              Al desarrollar soluciones de inteligencia artificial, la
              comprensión profunda de estas estructuras de datos fundamentales
              nos permite diseñar sistemas más eficientes y escalables. Un buen
              diseño de datos desde el principio puede significar la diferencia
              entre un sistema que funciona adecuadamente y uno que se vuelve
              inmanejable a medida que crece el volumen de datos.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Tema1',
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
