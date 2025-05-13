<template>
  <div class="curso-main-container pb-3">
    <BannerInterno></BannerInterno>
    <div class="container tarjeta tarjeta--blanca p-4 p-md-5 mb-5">
      <div class="titulo-principal color-acento-contenido">
        <div class="titulo-principal__numero"><span>2</span></div>
        <h1>Calidad y tratamiento de datos</h1>
      </div>
      <div class="row justify-content-center align-items-center mb-5">
        <div class="col-lg-9 my-lg-0 my-3">
          <div class="bg4 p-4">
            <p class="mb-0">
              La calidad y el tratamiento adecuado de los datos son pilares
              fundamentales para el éxito de cualquier proyecto de análisis o
              inteligencia artificial. En esta sección, se abordan las
              metodologías y técnicas necesarias para garantizar que los datos
              con los que trabajamos sean confiables, consistentes y útiles para
              los objetivos planteados.
            </p>
          </div>
        </div>
        <div class="col-lg-3 my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/34.png" alt="" />
        </div>
      </div>
      <Separador> </Separador>
      <div id="t_2_1" class="titulo-segundo color-acento-contenido">
        <h2>2.1 Características de calidad de datos</h2>
      </div>
      <div class="row justify-content-center align-items-center mb-4">
        <div class="col-auto my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/31.svg" alt="" />
        </div>
        <div class="col my-lg-0 my-3">
          <div class="bg6 p-3">
            <p class="mb-0">
              La calidad de los datos es un aspecto fundamental en el desarrollo
              de modelos de inteligencia artificial. Así como un chef no puede
              preparar un platillo exquisito con ingredientes en mal estado, un
              modelo de IA no puede proporcionar resultados confiables si se
              alimenta con datos de baja calidad. La famosa frase "<i
                ><b>garbage in, garbage out</b></i
              >" (entra basura, sale basura) resume perfectamente esta realidad
              en el campo del análisis de datos.
            </p>
          </div>
        </div>
      </div>
      <div class="row justify-content-center align-items-center mb-5">
        <div class="col-lg-9 my-lg-0 my-3">
          <p>
            La calidad de los datos se puede evaluar a través de múltiples
            dimensiones. La precisión es quizás la más evidente: los datos deben
            representar fielmente la realidad que intentan capturar. Por
            ejemplo, si estamos registrando la temperatura de un proceso
            industrial, necesitamos asegurarnos de que nuestros sensores estén
            correctamente calibrados y que las mediciones sean exactas.
          </p>
          <p>
            La completitud es otra dimensión estratégica. Los datos incompletos
            pueden llevar a conclusiones sesgadas o incorrectas. Imaginemos un
            estudio de satisfacción del cliente donde solo tenemos respuestas de
            usuarios muy satisfechos o insatisfechos: esto nos daría una visión
            distorsionada de la realidad, pues faltaría la información de
            aquellos clientes con opiniones moderadas.
          </p>
          <div class="bg6 p-3">
            <p class="mb-0">
              La consistencia de los datos implica que la información sea
              coherente a través de diferentes sistemas y registros. Por
              ejemplo, si un cliente aparece con diferentes direcciones en
              distintas bases de datos de la empresa, ¿cuál es la correcta? La
              falta de consistencia puede generar confusión y errores en el
              procesamiento de la información.
            </p>
          </div>
        </div>
        <div class="col-lg-3 my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/32.png" alt="" />
        </div>
      </div>
      <Separador> </Separador>
      <div id="t_2_2" class="titulo-segundo color-acento-contenido">
        <h2>2.2 Técnicas de extracción y filtrado</h2>
      </div>
      <div class="row justify-content-center align-items-center mb-5">
        <div class="col-lg-7 my-lg-0 my-3">
          <div class="bg8 p-4">
            <p class="mb-0">
              La extracción de datos es como la minería: debemos saber dónde
              buscar y qué herramientas utilizar para obtener la información
              valiosa. Este proceso involucra la identificación y recuperación
              de datos relevantes de diversas fuentes, que pueden incluir bases
              de datos relacionales, archivos de texto, hojas de cálculo,
              páginas web o incluso sensores IoT.
            </p>
          </div>
        </div>
        <div class="col-lg-5 my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/42.png" alt="" />
        </div>
      </div>
      <div class="row justify-content-center align-items-center mb-5">
        <div class="col-lg-5 my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/43.png" alt="" />
        </div>
        <div class="col-lg-7 my-lg-0 my-3">
          <div class="bg10 p-4">
            <p>
              Una de las técnicas más comunes de extracción es el
              <em>web scraping</em>, que permite obtener información
              estructurada de páginas web. Sin embargo, esta técnica debe
              utilizarse con responsabilidad, respetando los términos de
              servicio de los sitios web y las políticas de privacidad
              aplicables.
            </p>
            <p class="mb-0">
              El filtrado de datos es el proceso de eliminar o modificar datos
              que no cumplen con ciertos criterios de calidad o relevancia.
              Podemos clasificar las técnicas de filtrado en varias categorías
              según su propósito:
            </p>
          </div>
        </div>
      </div>
      <div class="row justify-content-center">
        <div class="col-lg-10">
          <div class="titulo-sexto color-acento-contenido">
            <h5>Tabla 2.</h5>
            <span
              >Tipos de filtrado de datos, objetivos, técnicas comunes y
              consideraciones.</span
            >
          </div>
          <div class="tabla-a color-acento-botones mb-5">
            <table>
              <caption>
                Fuente: OIT, 2024.
              </caption>
              <thead>
                <tr>
                  <th>Tipo de Filtrado</th>
                  <th>Objetivo</th>
                  <th>Técnicas Comunes</th>
                  <th>Consideraciones</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td>Limpieza</td>
                  <td>Eliminar errores y anomalías</td>
                  <td>Detección de <i>outliers</i>, corrección de formatos</td>
                  <td>Puede requerir validación manual</td>
                </tr>
                <tr>
                  <td>Reducción</td>
                  <td>Disminuir el volumen de datos</td>
                  <td>Muestreo, agregación</td>
                  <td>Riesgo de pérdida de información</td>
                </tr>
                <tr>
                  <td>Transformación</td>
                  <td>Convertir datos a formato útil</td>
                  <td>Normalización, codificación</td>
                  <td>Debe mantener la integridad de los datos</td>
                </tr>
                <tr>
                  <td>Enriquecimiento</td>
                  <td>Agregar información adicional</td>
                  <td class="fst-italic">Joins, lookup tables</td>
                  <td>Puede aumentar la complejidad</td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>
      <Separador> </Separador>
      <div id="t_2_3" class="titulo-segundo color-acento-contenido">
        <h2>2.3 Transformación e integración de datos</h2>
      </div>
      <div class="row justify-content-center mb-4">
        <div class="col my-lg-0 my-3">
          <p>
            La transformación de datos es como traducir un texto a diferentes
            idiomas: el significado debe mantenerse, aunque la forma cambie.
            Este proceso implica convertir los datos de su formato original a
            uno que sea más adecuado para el análisis o el modelado. Las
            transformaciones pueden ser tan simples como cambiar el formato de
            una fecha o tan complejas como aplicar cálculos matemáticos
            avanzados.
          </p>
          <p>
            Una transformación común es la normalización, que ajusta los valores
            numéricos a una escala común. Por ejemplo, si tenemos datos de
            ventas en diferentes monedas, necesitaremos convertirlos todos a una
            moneda común para poder compararlos adecuadamente. Otro ejemplo
            sería la estandarización de textos, asegurando que todas las cadenas
            de caracteres sigan el mismo formato (mayúsculas/minúsculas,
            tratamiento de espacios, etc.).
          </p>
        </div>
        <div class="col-auto my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/45.png" alt="" />
        </div>
      </div>
      <div class="row justify-content-center mb-5">
        <div class="col-lg-5 my-lg-0 my-3">
          <img class="img-a img-t" src="@/assets/curso/temas/44.png" alt="" />
        </div>
        <div class="col-lg-7 my-lg-0 my-3">
          <p>
            La integración de datos es el proceso de combinar datos de
            diferentes fuentes en una vista unificada y coherente. Este proceso
            puede ser particularmente desafiante cuando las fuentes tienen
            diferentes estructuras, formatos o niveles de calidad. Es como armar
            un rompecabezas donde las piezas provienen de diferentes cajas:
            necesitamos encontrar la forma de que encajen correctamente.
            <br /><br />Un aspecto clave de la integración es la resolución de
            conflictos. ¿Qué hacemos cuando diferentes fuentes proporcionan
            información contradictoria sobre el mismo elemento? Por ejemplo, si
            un cliente aparece con diferentes números de teléfono en distintas
            bases de datos, necesitamos establecer reglas claras para determinar
            cuál es la información correcta o más actualizada.
          </p>
          <p>
            La integración también debe considerar la temporalidad de los datos.
            Los datos históricos pueden ser valiosos para identificar tendencias
            y patrones, pero deben integrarse de manera que mantengan su
            contexto temporal. Por ejemplo, al analizar el rendimiento de
            ventas, necesitamos asegurarnos de que estamos comparando períodos
            equivalentes y considerando factores estacionales.
          </p>
          <p>
            El éxito en la transformación e integración de datos requiere un
            equilibrio entre la automatización y el criterio humano. Si bien
            muchos procesos pueden automatizarse, el conocimiento del dominio y
            el juicio experto son fundamentales para garantizar que las
            transformaciones sean significativas y que la integración produzca
            resultados útiles para el análisis posterior.
          </p>
        </div>
      </div>
      <div class="row justify-content-center align-items-center bg11 p-0">
        <div class="col-lg-5 my-lg-0 my-3 p-0">
          <img class="img-mov" src="@/assets/curso/temas/47.png" alt="" />
        </div>
        <div class="col-lg-7 my-lg-0 my-3">
          <div class="p-4 j1">
            <h5 class="text-white bg12 px-2">Cómo mitigar estos problemas</h5>
            <p class="mb-0">
              Para evitar que los datos contradictorios afecten el análisis y la
              toma de decisiones, es necesario implementar procesos robustos de
              validación, limpieza y unificación de datos. Asegurar la
              consistencia y la verificación continua es clave para obtener
              resultados precisos y confiables.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Tema2',
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
