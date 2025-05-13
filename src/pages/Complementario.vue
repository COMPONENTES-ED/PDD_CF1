<template>
  <div class="curso-main-container complementario">
    <BannerInterno
      icono="far fa-folder-open"
      titulo="Material complementario"
    ></BannerInterno>
    <div class="container tarjeta tarjeta--blanca p-4 p-md-5 mb-5">
      <div class="table-responsive">
        <table>
          <thead>
            <tr>
              <th colspan="3" scope="col">Tema</th>
              <th colspan="5" scope="col">Referencia APA del material</th>
              <th colspan="2" scope="col">Tipo</th>
              <th colspan="2" scope="col">Enlace</th>
            </tr>
          </thead>
          <tbody>
            <tr
              v-for="(item, index) in computedData"
              :key="'complementario-' + index"
            >
              <td
                class="text-start"
                colspan="3"
                scope="row"
                v-html="item.tema"
              ></td>
              <td
                class="text-start"
                colspan="5"
                scope="row"
                v-html="item.referencia"
              ></td>
              <td colspan="2" v-html="item.tipo"></td>
              <td colspan="2">
                <div class="complementario__enlaces">
                  <a
                    v-for="(link, linkIndex) of item.link"
                    :key="linkIndex"
                    class="complementario__btn"
                    :href="link"
                    target="_blank"
                    ><i class="fas fa-external-link-alt"></i
                  ></a>
                </div>
              </td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'MaterialComplementario',
  computed: {
    complementarioData() {
      return [
        {
          tema: '1. Fundamentos de datos y estructuras',
          referencia:
            'Ecosistema de Recursos Educativos Digitales SENA. (2023c, septiembre 5). <i>Ejemplo problemas en la recolección de la información</i>.',
          tipo: 'Video',
          link: 'https://www.youtube.com/watch?v=LOlsg6ZkdcA ',
        },
        {
          tema: '2. Calidad y tratamiento de datos',
          referencia:
            'Ecosistema de Recursos Educativos Digitales SENA. (2023b, septiembre 5). <i>Datos sucios</i>.',
          tipo: 'Video',
          link: 'https://www.youtube.com/watch?v=qf6MR4o58cs ',
        },
        {
          tema: '2. Calidad y tratamiento de datos',
          referencia:
            '<i>Limpiar datos de Excel, CSV, PDF y Hojas de cálculo de Google con el intérprete de datos. (s. f.). Tableau.</i>',
          tipo: 'Portal <i>web</i>',
          link:
            'https://help.tableau.com/current/pro/desktop/es-es/data_interpreter.htm ',
        },
        {
          tema: '2. Calidad y tratamiento de datos',
          referencia:
            'Ecosistema de Recursos Educativos Digitales SENA. (2022a, agosto 31). <i>Procesos y procedimientos para la gestión de calidad de la información</i>.',
          tipo: 'Video',
          link: 'https://www.youtube.com/watch?v=PeVlTP8qLhE ',
        },
        {
          tema: '2. Calidad y tratamiento de datos',
          referencia:
            'Ecosistema de Recursos Educativos Digitales SENA. (2023c, julio 25). <i>Procesamiento y análisis de datos</i>.',
          tipo: 'Video',
          link: 'https://www.youtube.com/watch?v=8OSIN2kdU5o ',
        },
        {
          tema: '3. Gestión de bases de datos',
          referencia:
            'Ecosistema de Recursos Educativos Digitales SENA. (2022b, octubre 11). <i>Conceptos y estructuras de las bases de datos</i>.',
          tipo: 'Video',
          link: 'https://www.youtube.com/watch?v=xUpr20u9dmc ',
        },
        {
          tema: '3. Gestión de bases de datos',
          referencia:
            'Ecosistema de Recursos Educativos Digitales SENA. (2023a, marzo 24). <i>Administración de bases de datos: Introducción</i>.',
          tipo: 'Video',
          link: 'https://www.youtube.com/watch?v=GL7CHwwPlKM ',
        },
        {
          tema: '4. Introducción a la Inteligencia Artificial',
          referencia:
            'Ecosistema de Recursos Educativos Digitales SENA. (2023b, marzo 24). <i>Inteligencia artificial en los datos.</i>',
          tipo: 'Video',
          link: 'https://www.youtube.com/watch?v=-hYXrGAUYAE ',
        },
      ]
    },
    computedData() {
      const data = this.complementarioData
      return data.map(item => {
        let nuevoLink = []
        if (item.link) {
          if (typeof item.link === 'string') {
            nuevoLink.push(item.link)
          } else {
            nuevoLink = item.link
          }
        } else if (item.descarga) {
          if (typeof item.descarga === 'string') {
            nuevoLink.push(this.obtenerLink(item.descarga))
          } else {
            item.descarga.forEach(link => {
              nuevoLink.push(this.obtenerLink(link))
            })
          }
        }
        return {
          ...item,
          link: nuevoLink,
        }
      })
    },
  },
}
</script>

<style lang="sass">
.complementario
  &__enlaces
    display: flex
    justify-content: center
    flex-wrap: wrap
    a
      margin: 0 5px
  &__btn
    font-size: 1.5em
    line-height: 1em
table
  width: calc(100% - 1px)
  min-width: 800px
  thead
    background-color: $color-sistema-e
    th
      border-color: $color-sistema-e
  th, td
    padding: 25px 20px
    text-align: center
</style>
