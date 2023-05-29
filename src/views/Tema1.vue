<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido(data-aos="fade-down-right")
      .titulo-principal__numero.text-white
        span 1
      h1 Interfaz y flujo de integración de Unity 3D
    p.mb-5(data-aos="fade-down-right") A continuación, se describen los pasos requeridos para la instalación de Unity 3D e información general de la forma de operar o utilizar algunas de sus funcionalidades básicas.
    img.mb-5(data-aos="fade-down-right")(src='@/assets/curso/tema1/imagen1.jpg')
    Separador
    #t_1_1.titulo-segundo.color-acento-contenido(data-aos="fade-down-right")
      h2 1.1 Instalación de Unity 3D
    p.mb-5(data-aos="fade-down-right") En este caso se utilizará la versión gratuita que puede descargar desde de 
      a.mb-4(:href="('https://unity.com/es')" target="_blank") 
        span.fuente-link https://unity.com/es
    .row.justify-content-center(data-aos="fade-down-right")
      .col-lg-10.col-11
        .tarjeta.fondo-1.p-3.mb-5
          .row.justify-content-center.align-items-center
            .col-3.col-sm-2.col-lg-1
              img(src="@/assets/curso/tema1/figura1.svg")
            .col
              .row.justify-content-between.align-items-center
                .col.mb-3.mb-sm-0
                  h3.mb-1 Unity Instalación
                  p.text-small En el siguiente documento puede consultar el detalle con los pasos de instalación, creación de Unity ID y el tipo de microjuego inicial.
                .col-sm-auto
                  a.boton.color-acento-botones(:href="obtenerLink('downloads/INSTALACION-PDF-2023.pdf')" target="_blank")
                    span Descargar
                    i.fas.fa-file-download
    Separador
    #t_1_2.titulo-segundo.color-acento-contenido(data-aos="fade-down-right")
      h2 1.2 Navegación en Unity 3D
    p(data-aos="fade-down-right") Después de finalizada la creación del proyecto se muestra la interfaz de Unity como se ve en la siguiente imagen.  
    p.mb-5(data-aos="fade-down-right") En dicha pantalla se puede ver el entorno 3D y las pestañas, desde allí se puede configurar la interfaz según la necesidad requerida.
    .titulo-sexto.color-acento-contenido(data-aos="fade-down-right")
      p.mb-0 #[b Figura 1]
      p.mb-0 Interfaz Unity
    figure.mb-5(data-aos="fade-down-right")
      img(src='@/assets/curso/tema1/imagen2.png', alt='Interfaz')
      figcaption  Nota. Pantalla principal proyecto Unity.
    p.mb-5(data-aos="fade-down-left") Además, puede configurar la interfaz de Unity 3D según la necesidad requerida a través de las siguientes opciones:
    AcordionA(data-aos="fade-down-right").mb-5(tipo="a" clase-tarjeta="tarjeta tarjeta--gris")
      .row.justify-content-around(titulo="Game")
        .col-md-5.mb-4.mb-md-0
          p En esta pestaña se ve el juego funcionando, para probarlo y verlo en ejecución se debe dar clic en el botón <em>play</em>. Cuando este botón está resaltado en azul indica que el juego está activo, tal como se muestra en la siguiente figura.
          a.boton.color-acento-botones.indicador__container(@click="modal1 = true")
            span Ampliar imagen
            i.fal.fa-magnifying-glass
            .indicador--click(v-if="mostrarIndicador")
          ModalA(:abrir-modal.sync="modal1")
            .row.justify-content-center
              .col-auto
                figure
                  img(src='@/assets/curso/tema1/imagen3.png', style="width: 850px")
                  figcaption Nota. Ejecución juego.
        .col-md-5
          figure
            img(src='@/assets/curso/tema1/imagen3.png')
          .div.fondo-2.p-2
            p.text-small.mb-0 Nota. Ejecución juego. 
      .row.justify-content-around(titulo="Scene")
        .col-md-5.mb-4.mb-md-0
          p Pestaña que permite configurar el escenario del videojuego, donde van a ir ubicados los elementos del mismo. Dichos elementos estarán listados en la pestaña de la izquierda llamada Hierarchy. Unity por defecto ubica dos elementos, cámara (Main Camera) e iluminación (Directional Light) como se muestra en la siguiente figura.
          a.boton.color-acento-botones.indicador__container(@click="modal2 = true")
            span Ampliar imagen
            i.fas.fa-magnifying-glass
            .indicador--click(v-if="mostrarIndicador")
          ModalA(:abrir-modal.sync="modal2")
            .row.justify-content-center
              .col-auto
                figure
                  img(src='@/assets/curso/tema1/imagen4.png', style="width: 850px")
                  figcaption Nota. Opciones pestaña <em>Scene</em>.
        .col-md-5
          figure
            img(src='@/assets/curso/tema1/imagen4.png')
          .div.fondo-2.p-2
            p.text-small.mb-0 Nota. Opciones pestaña <em>Scene</em>.
      .row.justify-content-around(titulo="Inspector")
        .col-md-11.mb-4.mb-md-0
          p Al lado derecho se muestra la pestaña Inspector, en la cual se pueden modificar los atributos y propiedades de cada elemento, como se muestra en las siguientes figuras:
        .row.justify-content-around
          .col-md-5
            figure
              img(src='@/assets/curso/tema1/imagen5.png')
            .div.fondo-2.p-2
              p.text-small.mb-0 Nota. Pestaña Inspector. 
          .col-md-5
            figure
              img(src='@/assets/curso/tema1/imagen6.png')
            .div.fondo-2.p-2
              p.text-small.mb-0 Nota. Opciones Inspector.
      .row.justify-content-around(titulo="Project")
        .col-md-11.mb-4.mb-md-0
          p En la parte inferior izquierda se encuentra la pestaña Project, que es de suma importancia, pues allí se agregarán archivos externos a Unity como sonidos, texturas, imágenes, entre otros; los cuales pueden anexarse simplemente arrastrándolos, dando clic en la pestaña Assets - crear como se muestra en la siguiente figura.
        .row.justify-content-around
          .col-md-5
            figure
              img(src='@/assets/curso/tema1/imagen7.png')
            .div.fondo-2.p-2
              p.text-small.mb-0 Nota. Opciones pestaña <em>Project</em>.
          .col-md-5
            figure
              img(src='@/assets/curso/tema1/imagen8.png')
            .div.fondo-2.p-2
              p.text-small.mb-0 Nota. Opciones pestaña <em>Project - Create</em>.
    Separador
    #t_1_3.titulo-segundo.color-acento-contenido(data-aos="fade-down-right")
      h2 1.3 Escenario y ventanas de Unity 3D
    p.mb-5(data-aos="fade-down-right") Se puede modificar la vista y tamaño de la escena por medio de las siguientes alternativas:
    AcordionA(data-aos="fade-down-right")(tipo="a" clase-tarjeta="tarjeta tarjeta--gris")
      .row.justify-content-around(titulo="Tamaño escena")
        .col-md-5.mb-4.mb-md-0
          p La ventana y vista de la escena se puede ampliar arrastrándola a partir de sus bordes, como se identifica en la siguiente figura.
          p En el escenario hay 3 ejes, alto, ancho y profundidad, que se indican en la parte superior derecha con las letras X, Y, Z. 
          p Al dar clic derecho con el mouse se puede rotar la vista, además de que si se mantiene oprimido y se presiona las teclas WASD se podrá mover por el escenario como si se tratase de un videojuego en primera persona.
          a.boton.color-acento-botones.indicador__container(@click="modal3 = true")
            span Ampliar imagen
            i.fas.fa-magnifying-glass
            .indicador--click(v-if="mostrarIndicador")
          ModalA(:abrir-modal.sync="modal3")
            .row.justify-content-center
              .col-auto
                figure
                  img(src='@/assets/curso/tema1/imagen9.png', style="width: 850px")
                  figcaption Nota. Identificación bordes cambio de tamaño 
        .col-md-5
          figure
            img(src='@/assets/curso/tema1/imagen9.png')
          .div.fondo-2.p-2
            p.text-small.mb-0 Nota. Identificación bordes cambio de tamaño escena.
      .row.justify-content-around(titulo="Zoom")
        .col-md-5.mb-4.mb-md-0
          p Al girar la rueda del mouse se puede hacer zoom o acercamiento, al presionarla y mantenerla oprimida, el cursor toma forma de mano, lo que permite mover la vista del escenario, como se puede ver en la siguiente figura.
          a.boton.color-acento-botones.indicador__container(@click="modal4 = true")
            span Ampliar imagen
            i.fas.fa-magnifying-glass
            .indicador--click(v-if="mostrarIndicador")
          ModalA(:abrir-modal.sync="modal4")
            .row.justify-content-center
              .col-auto
                figure
                  img(src='@/assets/curso/tema1/imagen10.png', style="width: 850px")
                  figcaption Nota. Movimiento escenario - Zoom.
        .col-md-5
          figure
            img(src='@/assets/curso/tema1/imagen10.png')
          .div.fondo-2.p-2
            p.text-small.mb-0 Nota. Movimiento escenario - Zoom.
      .row.justify-content-around(titulo="Vista")
        .col-md-5.mb-4.mb-md-0
          p Si se mantiene la tecla alt + clic izquierdo se puede girar la vista en torno al punto central de la misma, como se muestra en la siguiente figura.
          a.boton.color-acento-botones.indicador__container(@click="modal5 = true")
            span Ampliar imagen
            i.fas.fa-magnifying-glass
            .indicador--click(v-if="mostrarIndicador")
          ModalA(:abrir-modal.sync="modal5")
            .row.justify-content-center
              .col-auto
                figure
                  img(src='@/assets/curso/tema1/imagen11.png', style="width: 850px")
                  figcaption Nota. Movimiento escenario - vista. 
        .col-md-5
          figure
            img(src='@/assets/curso/tema1/imagen11.png')
          .div.fondo-2.p-2
            p.text-small.mb-0 Nota. Movimiento escenario - vista.

</template>

<script>
export default {
  name: 'Tema1',
  components: {},
  data: () => ({
    // variables de vue
    modal1: false,
    modal2: false,
    modal3: false,
    modal4: false,
    modal5: false,
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
