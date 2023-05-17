<template lang="pug">
.curso-main-container.introduccion
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
  
    .titulo-principal.color-acento-contenido(data-aos="fade-down-right")
      .titulo-principal__numero.text-white
        span
          i.fas.fa-info
      h1 Introducción
    .div(data-aos="fade-down-right")
      img(src='@/assets/curso/intro/imagen.png')
    .bloque-texto-b.fondo-bloque.p-4.my-5(data-aos="fade-down-right")
      .bloque-texto-b__texto
        p.mb-0 En este componente se explicará la interfaz de Unity, su instalación, navegación y las ventanas que serán de importancia para el desarrollo de proyectos de videojuegos. También encontrará información sobre la  importación de objetos 3D, desde Blender e integración de Asset Store de Unity y cómo componer escenarios propios.
        br
        br 
        p De esta manera se podrá evidenciar la importancia del uso de la iluminación en los videojuegos y cuáles son los tipos de luces. Asimismo, se explicará la posición de las cámaras, para qué sirven y cómo se pueden tomar decisiones para realizar las interfaces de los videojuegos, y cómo realizar una propia.
</template>

<script>
export default {
  name: 'Introduccion',
  data: () => ({
    // variables de vue
  }),
}
</script>

<style lang="sass"></style>
