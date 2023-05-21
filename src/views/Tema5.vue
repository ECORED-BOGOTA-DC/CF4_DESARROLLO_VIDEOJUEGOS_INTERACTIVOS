<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido(data-aos="fade-down")
      .titulo-principal__numero.text-white
        span 5
      h1 Cámaras
    p.mb-4(data-aos="fade-down-left") La cámara principal es la que se utiliza por defecto, que es la que muestra el visor de la escena general, la cual se puede rotar e interactuar con ella, desde la posición de perspectiva y el modo ortográfico, con el gizmo ubicado en la parte superior derecha se puede observar que tiene unos ejes y un cuadro amarillo. Con ellos clicando encima se puede navegar perspectiva y vista ortogonal, esto permite poder diseñar de una forma más cómoda y precisa, como se muestra la siguiente figura.
    .titulo-sexto.color-acento-contenido.mb-4(data-aos="fade-down-right")
      p.mb-0 #[b #[i Figura 16]]
      p.mb-0 Vista ortogonal y perspectiva
    figure.mb-5(data-aos="fade-down-left")
      img(src='@/assets/curso/tema5/imagen1.jpg')
      figcaption  Nota. Ejemplo vista ortogonal y perspectiva.
    .row.justify-content-center(data-aos="fade-down-right")
      .col-lg-10.col-11
        .tarjeta.fondo-1.p-3
          .row.justify-content-center.align-items-center
            .col-3.col-sm-2.col-lg-1
              img(src="@/assets/curso/tema1/figura1.svg")
            .col
              .row.justify-content-between.align-items-center
                .col.mb-3.mb-sm-0
                  h3.mb-1 Unity Cámara
                  p.text-small Información adicional relacionada con las propiedades de cámaras, ejemplos de perspectivas, entre otros, puede consultarla en el siguiente documento.
                .col-sm-auto
                  a.boton.color-acento-botones(:href="obtenerLink('downloads/CAMARA-PDF-2023.pdf')" target="_blank")
                    span Descargar
                    i.fas.fa-file-download   
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
