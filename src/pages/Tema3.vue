<template>
  <div class="curso-main-container pb-3">
    <BannerInterno></BannerInterno>
    <div class="container tarjeta tarjeta--blanca p-4 p-md-5 mb-5">
      <div class="titulo-principal color-acento-contenido">
        <div class="titulo-principal__numero"><span>3</span></div>
        <h1>Gestión de bases de datos</h1>
      </div>
      <div
        class="bloque-texto-g bloque-texto-g--inverso color-acento-contenido p-3 p-sm-4 p-md-5"
      >
        <div
          class="bloque-texto-g__img"
          :style="{
            'background-image': `url(${require('@/assets/curso/temas/48.png')})`,
          }"
        ></div>
        <div class="bloque-texto-g__texto p-4">
          <p class="mb-0">
            La gestión efectiva de bases de datos representa un componente
            central en la infraestructura de cualquier sistema de información
            moderno. En este capítulo, se explorarán los diferentes tipos de
            bases de datos, sus características distintivas y las mejores
            prácticas para su administración y optimización.
          </p>
        </div>
      </div>
      <Separador> </Separador>
      <div id="t_3_1" class="titulo-segundo color-acento-contenido">
        <h2>3.1 Bases de datos relacionales y no relacionales</h2>
      </div>
      <div class="row justify-content-center mb-5">
        <div class="col-lg-5 my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/59.png" alt="" />
        </div>
        <div class="col-lg-7 my-lg-0 my-3">
          <div class="bg4 p-4 h-100 j1">
            <p>
              En el ecosistema moderno de gestión de datos, nos encontramos
              principalmente con dos grandes familias de bases de datos: las
              relacionales y las no relacionales (NoSQL). Cada una tiene sus
              propias fortalezas y casos de uso ideales, y comprender sus
              diferencias es fundamental para tomar decisiones acertadas en el
              diseño de sistemas de datos.
            </p>
            <p class="mb-0">
              Para visualizar mejor las diferencias fundamentales entre estos
              dos tipos de bases de datos, observemos la siguiente
              representación gráfica. Como se ilustra en la infografía, mientras
              las bases de datos relacionales se caracterizan por su estructura
              rígida y garantías ACID, las bases de datos NoSQL destacan por su
              flexibilidad y escalabilidad. Esta distinción es muy importante al
              momento de seleccionar el tipo de base de datos más adecuado para
              nuestras necesidades específicas. Por ejemplo, si necesitamos
              mantener la integridad referencial en transacciones financieras,
              una base de datos relacional sería la elección óptima. En cambio,
              si estamos manejando datos de redes sociales con estructuras
              variables y alto volumen de escrituras, una base de datos NoSQL
              podría ser más apropiada.
            </p>
          </div>
        </div>
      </div>
      <div class="row justify-content-center mb-5">
        <div class="col-auto">
          <div class="titulo-sexto color-acento-contenido">
            <h5>Figura 1.</h5>
            <span>Tipos de bases de datos</span>
          </div>
          <img
            class="img-a img-t mb-2"
            src="@/assets/curso/temas/60.svg"
            alt="La Figura 1 se denomina «Tipos de bases de datos» y presenta un comparativo entre las bases de datos relacionales y las NoSQL."
          />
          <figcaption>Fuente. OIT, 2024.</figcaption>
        </div>
      </div>
      <div class="row justify-content-center mb-5 pb-3">
        <div class="col-lg-5 my-lg-0 my-3">
          <div class="p-3 h-100 j1">
            <p class="mb-0">
              Ahora bien, las bases de datos relacionales han sido el pilar de
              la gestión de datos durante décadas. Se basan en el modelo
              relacional, donde los datos se organizan en tablas con filas y
              columnas claramente definidas. La fortaleza de este modelo radica
              en su capacidad para mantener la integridad de los datos y
              establecer relaciones claras entre diferentes entidades. Cuando
              necesitamos garantizar la consistencia de las transacciones y
              mantener relaciones complejas entre datos, las bases de datos
              relacionales son la opción más segura.
            </p>
          </div>
        </div>
        <div class="col-lg-3 my-lg-0 my-3 j1">
          <img class="img-a img-t" src="@/assets/curso/temas/61.png" alt="" />
        </div>
        <div class="col-lg-4 my-lg-0 my-3">
          <div class="bg13 brad p-2 px-3 h-100 j1">
            <p class="mb-0">
              Por otro lado, las bases de datos NoSQL surgieron como respuesta a
              las necesidades de la era del big data y la web moderna. Ofrecen
              mayor flexibilidad en cuanto a la estructura de los datos y mejor
              escalabilidad horizontal. No requieren un esquema fijo, lo que las
              hace ideales para datos semi-estructurados o cuando la estructura
              de los datos puede cambiar con frecuencia.
            </p>
          </div>
        </div>
      </div>
      <Separador> </Separador>
      <div id="t_3_2" class="titulo-segundo color-acento-contenido">
        <h2>3.2 Operaciones CRUD y consultas básicas</h2>
      </div>
      <div class="row justify-content-center mb-5">
        <div class="col-lg-5 my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/62.png" alt="" />
          <figcaption>Tomado de lab.wallarm.com</figcaption>
        </div>
        <div class="col-lg-7 my-lg-0 my-3">
          <div class="bg4 p-4 h-100 j1">
            <p>
              <b>Las operaciones CRUD (Create, Read, Update, Delete)</b> son de
              alta relevancia para interactuar con los datos almacenados en
              cualquier sistema de base de datos. La implementación de estas
              operaciones varía según el tipo de base de datos, pero los
              principios básicos permanecen constantes.
            </p>
            <p>
              En el contexto de bases de datos relacionales, estas operaciones
              se realizan mediante SQL (Structured Query Language). Las
              consultas SELECT permiten recuperar datos específicos, mientras
              que INSERT, UPDATE y DELETE se utilizan para modificar los
              registros existentes. La potencia de SQL radica en su capacidad
              para realizar consultas complejas que combinan datos de múltiples
              tablas y aplican criterios de filtrado y agregación.
            </p>
            <p>
              Para las bases de datos NoSQL, las operaciones CRUD se implementan
              de manera diferente según el tipo específico de base de datos. Por
              ejemplo, en una base de datos documental como MongoDB, se trabaja
              con documentos JSON que pueden tener estructura variable, y las
              operaciones se realizan mediante métodos específicos de la API de
              la base de datos.
            </p>
          </div>
        </div>
      </div>
      <Separador> </Separador>
      <div id="t_3_3" class="titulo-segundo color-acento-contenido">
        <h2>3.3 Gestión y optimización de bases de datos</h2>
      </div>
      <div class="row justify-content-center mb-5">
        <div class="col-lg-7 my-lg-0 my-3">
          <div class="bg14 p-4 h-100 j1">
            <p>
              La gestión efectiva de bases de datos va más allá de simplemente
              almacenar y recuperar información. Implica un conjunto de
              prácticas y técnicas para asegurar el rendimiento, la
              disponibilidad y la integridad de los datos. La optimización es un
              proceso continuo que debe adaptarse a las cambiantes necesidades
              del sistema.
            </p>
            <p>
              Un aspecto esencial de la optimización es el diseño e
              implementación de índices. Los índices son estructuras de datos
              adicionales que mejoran la velocidad de las operaciones de
              búsqueda, pero tienen un costo en términos de espacio de
              almacenamiento y rendimiento de escritura. La decisión de qué
              campos indexar debe basarse en un análisis cuidadoso de los
              patrones de acceso a los datos.
            </p>
          </div>
        </div>
        <div class="col-lg-5 my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/63.png" alt="" />
        </div>
      </div>
      <div class="row justify-content-center mb-5">
        <div class="col-lg-5 my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/64.png" alt="" />
        </div>
        <div class="col-lg-7 my-lg-0 my-3">
          <p>
            El monitoreo del rendimiento es una parte fundamental de la gestión
            de bases de datos. Es necesario prestar atención a métricas como el
            tiempo de respuesta de las consultas, el uso de recursos del sistema
            y los patrones de acceso a los datos. Las herramientas de monitoreo
            identifican cuellos de botella y oportunidades de optimización.
          </p>
          <p>
            La seguridad es otro aspecto que no puede descuidarse. Esto incluye
            la gestión de usuarios y permisos, la encriptación de datos
            sensibles y la implementación de políticas de respaldo y
            recuperación. En el contexto de la inteligencia artificial, donde
            frecuentemente se trabaja con datos sensibles o personales, la
            seguridad adquiere una importancia aún mayor.
          </p>
          <p>
            La escalabilidad es un factor clave en la gestión de grandes
            volúmenes de datos. Los sistemas de bases de datos deben ser
            diseñados para adaptarse al crecimiento futuro, ya sea a través de
            escalabilidad vertical (ampliando los recursos de un único servidor)
            o horizontal (distribuyendo la carga entre varios servidores). Las
            estrategias de particionamiento y replicación son fundamentales para
            manejar grandes cantidades de datos de forma eficiente.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Tema3',
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
