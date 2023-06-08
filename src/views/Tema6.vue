<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido(data-aos="fade-down")
      .titulo-principal__numero.text-white
        span 6
      h1 Efectos visuales
    p.mb-4(data-aos="fade-down-left") Hacen que las acciones durante el juego se destaquen mucho más, dándole más impacto visual a las escenas, por ejemplo, en un combate los golpes se hacen más visibles con efectos, el piso al combatir puede botar partículas, si hay un disparo se puede generar humo, puede haber un entorno con neblina, lluvia, fuego, entre muchos más.  La siguiente figura muestra un ejemplo:
    .titulo-sexto.color-acento-contenido.mb-4(data-aos="fade-down-right")
      p.mb-0 #[b Figura 17]
      p.mb-0 Explosion Hollow Knight
    figure.mb-5(data-aos="fade-down-left")
      img(src='@/assets/curso/tema6/imagen1.jpg')
      figcaption Nota. Ejemplo efecto visual. <em>Interfaceingame</em> (s.f.).

</template>

<script>
export default {
  name: 'Tema6',
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
