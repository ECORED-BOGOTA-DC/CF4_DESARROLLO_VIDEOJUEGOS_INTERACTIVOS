<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero.text-white
        span 3
      h1 Componer los escenarios (personajes, <em>props</em>, fondos)
    figure.mb-5(data-aos="fade-down-left")
      img(src='@/assets/curso/tema3/imagen1.png')
    p.mb-5(data-aos="fade-down-right") Para la composición de escenarios Unity cuenta con herramientas que facilitan su desarrollo, como es el caso de la herramienta editor de terrenos, en la cual se pueden asignar texturas y color a los mismos. Para usar la herramienta crear terrenos se sigue la ruta de <em>GameObject – 3D Object – Terrain</em>, como se muestra a continuación:
    .titulo-sexto.color-acento-contenido(data-aos="fade-down-right")
      p.mb-0 #[b #[i Figura 11]]
      p.mb-0 Terrain
    figure.mb-5(data-aos="fade-down-left")
      img(src='@/assets/curso/tema3/imagen2.png')
      figcaption Nota. Opción crear <em>Terrain</em>.
    p.mb-5(data-aos="fade-down-right") Al hacerlo se forma un plano de recuadros en el escenario, ahora en el panel de Inspector se puede configurar el terreno, como se muestra en la siguiente figura.
    .titulo-sexto.color-acento-contenido(data-aos="fade-down-right")
      p.mb-0 #[b #[i Figura 12]]
      p.mb-0 Configurar terreno
    figure.mb-5(data-aos="fade-down-left")
      img(src='@/assets/curso/tema3/imagen3.png')
      figcaption Nota. Opciones de configuración terreno.
    .row.justify-content-center.mb-4(data-aos="fade-down-right")
      .col-lg-10.col-11
        .tarjeta.fondo-1.p-3.mb-5
          .row.justify-content-center.align-items-center
            .col-3.col-sm-2.col-lg-1
              img(src="@/assets/curso/tema1/figura1.svg")
            .col
              .row.justify-content-between.align-items-center
                .col.mb-3.mb-sm-0
                  h3.mb-1 Unity Terrenos
                  p.text-small En el siguiente documento puede consultar información complementaria relacionada con las propiedades de terreno.
                .col-sm-auto
                  a.boton.color-acento-botones(:href="obtenerLink('downloads/prueba.pdf')" target="_blank")
                    span Descargar
                    i.fas.fa-file-download
    p.text-center.mb-4(data-aos="fade-down-right") A continuación, puede visualizar la integración de assets en Unity para la creación de escenarios.
    figure(data-aos="fade")
      .video
        iframe(width="560" height="315" src="https://www.youtube.com/embed/Zj0CCgboE2o" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)

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
