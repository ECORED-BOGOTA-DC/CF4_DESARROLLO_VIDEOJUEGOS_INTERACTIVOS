<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    p.mb-5 Este componente formativo abordó todo lo que tiene que ver con el manejo de la interfaz de Unity, su instalación, la formación de navegación,  las ventanas que son importantes a la hora de crear escenarios, propios, entre otros temas indispensables e la hora de desarrollar los proyectos de videojuegos. A continuación, podrá observar el esquema de temas que componen esta temática.
    .row.justify-content-center
      .col-lg-8.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis.svg", alt="alt")
    .row.justify-content-center
      .col-auto
        a.anexo.mb-4(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
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
