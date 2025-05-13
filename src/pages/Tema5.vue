<template>
  <div class="curso-main-container pb-3">
    <BannerInterno></BannerInterno>
    <div class="container tarjeta tarjeta--blanca p-4 p-md-5 mb-5">
      <div class="titulo-principal color-acento-contenido">
        <div class="titulo-principal__numero"><span>5</span></div>
        <h1>Conclusiones</h1>
      </div>
      <div class="bloque-texto-g color-secundario p-3 p-sm-4 p-md-5">
        <div
          class="bloque-texto-g__img"
          :style="{
            'background-image': `url(${require('@/assets/curso/temas/73.png')})`,
          }"
        ></div>
        <div class="bloque-texto-g__texto p-4">
          <p class="mb-0">
            El procesamiento de datos para modelos de inteligencia artificial
            requiere una comprensión profunda y holística que va desde los
            fundamentos más básicos hasta las aplicaciones más avanzadas. A lo
            largo de este componente formativo, se exploró cómo los datos, en su
            forma más elemental, se transforman en estructuras complejas que
            alimentan los sistemas de IA modernos.<br /><br />
            La gestión efectiva de estos datos, desde su recolección hasta su
            procesamiento final, resulta fundamental para el éxito de cualquier
            proyecto de inteligencia artificial. <br /><br />La convergencia
            entre las estructuras de datos tradicionales, los sistemas de
            gestión de bases de datos y las tecnologías emergentes de IA nos
            muestra un panorama en constante evolución. La calidad de los datos,
            su tratamiento adecuado y la selección de las herramientas
            apropiadas no son simplemente pasos en un proceso, sino elementos
            críticos que determinan la eficacia de los modelos de IA.
            <br /><br />A medida que avanzamos hacia un futuro cada vez más
            dependiente de los datos y la inteligencia artificial, la capacidad
            para manejar estos conceptos fundamentales se vuelve no solo
            deseable sino indispensable para cualquier persona que trabaja en el
            campo de la tecnología.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'Tema5',
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
