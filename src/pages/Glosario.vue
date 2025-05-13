<template>
  <div class="curso-main-container glosario">
    <BannerInterno icono="fas fa-atlas" titulo="Glosario"></BannerInterno>
    <div class="container tarjeta tarjeta--blanca p-4 p-md-5 mb-5">
      <div
        v-for="letra in orderedData"
        :key="'letra-' + letra.letra"
        class="glosario__letra-item mb-2"
      >
        <div class="glosario__letra-item__letra me-4">
          <div class="glosario__letra-item__letra__icono">
            <span>{{ letra.letra }}</span>
          </div>
        </div>
        <div class="glosario__letra-item__texto">
          <p
            v-for="termino in letra.terminos"
            :key="termino.termino"
            class="mb-3"
          >
            <strong><i class="lista-ul__vineta"></i></strong
            ><strong v-html="termino.terminoHtml || termino.termino"> </strong
            ><strong>: </strong><span v-html="termino.significado"></span>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import plantillaMixins from '@/js/plantillaMixins'
export default {
  name: 'Glosario',
  mixins: [plantillaMixins],
  data() {
    return {
      glosarioData: [
        {
          termino: 'ACID',
          significado:
            'Acrónimo de Atomicidad, Consistencia, Aislamiento y Durabilidad; propiedades que garantizan que las transacciones en una base de datos sean fiables.',
        },
        {
          termino: 'Algoritmo',
          significado:
            'Conjunto ordenado y finito de operaciones sistemáticas que permite hacer un cálculo y hallar la solución de un problema específico.',
        },
        {
          termino: 'Base de datos',
          significado:
            'Sistema organizado para recopilar, almacenar y gestionar datos de manera estructurada y eficiente.',
        },
        {
          termino: 'CRUD',
          significado:
            '<i>Acrónimo de Create, Read, Update, Delete;</i> operaciones básicas que se pueden realizar sobre datos almacenados.',
        },
        {
          termino: '<i>Dataset</i>',
          significado:
            'Conjunto de datos organizados y formateados de manera específica para su uso en análisis o entrenamiento de modelos.',
        },
        {
          termino: 'Datos estructurados',
          significado:
            'Información que está organizada en un formato predefinido y fácilmente procesable por máquinas, típicamente en tablas con filas y columnas.',
        },
        {
          termino: 'ETL',
          significado:
            '<i>Extract, Transform, Load </i>(Extraer, Transformar, Cargar); proceso que permite a las organizaciones mover datos desde múltiples fuentes, reformatearlos y limpiarlos, y cargarlos en otra base de datos.',
        },
        {
          termino: 'Estructura de datos',
          significado:
            'Forma particular de organizar datos en una computadora para que puedan ser utilizados de manera eficiente.',
        },
        {
          termino: 'Indexación',
          significado:
            'Proceso de crear estructuras de datos adicionales que mejoran la velocidad de recuperación de información en una base de datos.',
        },
        {
          termino: 'Inteligencia Artificial',
          significado:
            'Campo de la informática que busca crear sistemas capaces de aprender y resolver problemas de manera similar a como lo haría un ser humano.',
        },
        {
          termino: 'JSON',
          significado:
            '<i>JavaScript Object Notation; </i>formato ligero de intercambio de datos, fácil de leer y escribir para humanos y máquinas.',
        },
        {
          termino: '<i>Machine Learning</i>',
          significado:
            'Rama de la inteligencia artificial que se centra en el desarrollo de técnicas que permiten que las computadoras aprendan y mejoren a partir de la experiencia.',
        },
        {
          termino: 'Metadata',
          significado:
            'Datos que proporcionan información sobre otros datos, describiendo su contenido, calidad, condición y otras características.',
        },
        {
          termino: 'NoSQL',
          significado:
            'Tipo de base de datos que no utiliza el esquema tradicional de tablas relacionales, permitiendo mayor flexibilidad y escalabilidad.',
        },
        {
          termino: 'Normalización',
          significado:
            'Proceso de organizar los datos en una base de datos para reducir la redundancia y mejorar la integridad de los datos.',
        },
        {
          termino: 'Pipeline de datos',
          significado:
            'Conjunto de procesos y herramientas que permiten mover datos desde una fuente hacia un destino, realizando transformaciones en el camino.',
        },
        {
          termino: '<i>Query</i>',
          significado:
            'Consulta o petición específica para recuperar información de una base de datos.',
        },
        {
          termino: '<i>Schema</i>',
          significado:
            'Estructura que define cómo se organizan los datos en una base de datos, incluyendo tablas, campos y relaciones.',
        },
        {
          termino: 'SQL',
          significado:
            '<i>Structured Query Language; </i>lenguaje estándar para gestionar y manipular bases de datos relacionales.',
        },
        {
          termino: 'Validación de datos',
          significado:
            'Proceso de asegurar que los datos cumplan con ciertos criterios de calidad y formato antes de ser utilizados en análisis o procesamiento posterior.',
        },
      ],
    }
  },
  computed: {
    orderedData() {
      const newGlosarioData = [...this.glosarioData]
      newGlosarioData.forEach(element => {
        element.significado =
          element.significado.charAt(0).toLowerCase() +
          element.significado.slice(1)
      })

      const sortedData = [...newGlosarioData].reduce((r, e) => {
        const letra = this.quitarAcentos(e.termino.toLowerCase())[0]
        if (!r[letra]) r[letra] = { letra, terminos: [e] }
        else r[letra].terminos.push(e)
        return r
      }, {})

      const soloLetras = Object.keys(sortedData).sort()
      const newSortedData = []

      soloLetras.forEach(element => {
        const letraObj = sortedData[element]
        let terminos = letraObj.terminos

        if (terminos.length > 1) {
          const terminosOrdenados = []
          const soloTerminos = letraObj.terminos
            .map(termObj => termObj.termino)
            .sort((a, b) => {
              const an = this.quitarAcentos(a).toLowerCase()
              const bn = this.quitarAcentos(b).toLowerCase()
              if (an < bn) return -1
              if (bn < an) return 1
              return 0
            })
          soloTerminos.forEach(term => {
            terminosOrdenados.push(
              terminos.find(termino => termino.termino === term),
            )
          })
          terminos = terminosOrdenados
        }
        newSortedData.push({
          letra: letraObj.letra.toUpperCase(),
          terminos: terminos,
        })
      })
      return newSortedData
    },
  },
}
</script>

<style lang="sass">
.glosario
  &__letra-item
    display: flex
    &__texto
      padding-top: 5px
    &__letra
      &__icono
        width: 32px
        height: 32px
        position: relative
        line-height: 1em
        border-radius: 50%
        background-color: $color-sistema-d

        span
          position: absolute
          left: 50%
          top: 50%
          transform: translate(-50%,-50%)
          font-size: 1.1em
          font-weight: $base-black-font-weight
</style>
