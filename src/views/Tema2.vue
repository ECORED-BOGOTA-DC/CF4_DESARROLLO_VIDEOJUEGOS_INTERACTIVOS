<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido(data-aos="fade-down-right")
      .titulo-principal__numero.text-white
        span 2
      h1 Unity 3D importar elementos 3D - <em>assets</em>
    figure(data-aos="fade-down-left")
      img(src='@/assets/curso/tema2/imagen1.png')
      figcaption <em>Unity Asset Store</em>
    p.my-5(data-aos="fade-down-right") A continuación, se describe el funcionamiento de algunas de las opciones de Unity 3D a través de ejemplos con su correspondiente explicación.
    .cajon.color-primario.fondo-cajon.p-4.mb-4(data-aos="fade-down-right")
      .row.justify-content-center.align-items-center
        .col-lg-1.col-md-2.col-sm2.col-3
          img(src='@/assets/curso/tema2/figura1.svg')
        .col-lg-11.col-md-10.col-sm2.col-9
          p.mb-0 Para este ejemplo se creará un cubo y se posicionará en el escenario. La ruta es la siguiente, en el menú principal situado en la parte superior se selecciona la opción GameObject, como se puede ver en la siguiente figura.
    .row.justify-content-center
      .col-lg-8.col-md-10.col-sm-11.col-12
        .titulo-sexto.color-acento-contenido(data-aos="fade-down-right")
          p.mb-0 #[b Figura 2]
          p.mb-0 Menú GameObject
        figure.my-4(data-aos="fade-down-left")
          img(src='@/assets/curso/tema2/imagen2.svg')
          figcaption Nota. Opción menú GameObject.
    p.mb-5(data-aos="fade-down-right") Después se selecciona la opción Cube del menú 3D Object, como se muestra en la siguiente figura.
    .titulo-sexto.color-acento-contenido.mb-4(data-aos="fade-down-right")
      p.mb-0 #[b Figura 3]
      p.mb-0 Crear cubo
    figure.mb-4(data-aos="fade-down-left")
      img(src='@/assets/curso/tema2/imagen3.svg')
      figcaption Nota. Opción menú crear cubo.
    p.mb-5(data-aos="fade-down-right") Una vez hecho esto, en el escenario se incluirá un cubo. Para mover los objetos en el escenario, en la parte superior izquierda se encuentran 3 iconos: mover, rotar y escalar, como se resalta en la siguiente figura.
    .titulo-sexto.color-acento-contenido.mb-4(data-aos="fade-down-right")
      p.mb-0 #[b Figura 4]
      p.mb-0 Mover, rotar, escalar
    figure.mb-4(data-aos="fade-down-left")
      img(src='@/assets/curso/tema2/imagen4.svg')
      figcaption Nota. Opciones iconos mover, rotar, escalar.
    .tarjeta.tarjeta--azul.p-4.mb-5
      SlyderA(tipo="b")
        .row.justify-content-center.mt-4
          .col-lg-4.mb-4.mb-md-0
            h4 Botón mover
            p Cuando se selecciona un objeto en el escenario, habiendo pulsado el botón mover, en el objeto se mostrarán 3 flechas que representan los 3 ejes mencionados anteriormente. Si se da clic sostenido en dichas flechas y se mueve el mouse se traslada en línea recta el objeto en el escenario en el eje de coordenadas seleccionado, como se representa en la siguiente figura.
        
          .col-lg-7
            figure
              img(src='@/assets/curso/tema2/imagen5.png', alt='Botón mover')
              figcaption Nota. Botón mover.
        .row.justify-content-center.mt-4
          .col-lg-4.mb-4.mb-md-0
            h4 Botón mover - dos ejes
            p Si se quiere mover el objeto en dos ejes al mismo tiempo se da clic en los recuadros internos del objeto, el cuadro selecciona esos dos ejes que componen el cuadro pequeño interno, como se muestra en la siguiente figura.
          .col-lg-7
            figure
              img(src='@/assets/curso/tema2/imagen6.png', alt='Botón mover - dos ejes')
              figcaption Nota. Botón mover - dos ejes.
        .row.justify-content-center.mt-4
          .col-lg-4.mb-4.mb-md-0
            h4 Botón rotar o girar
            p Cuando se activa el botón rotar y se selecciona un objeto, este se ve envuelto por líneas circundantes en sus respectivos ejes y una circundante global, como puede evidenciarse en la siguiente figura.
            p Al dar clic en alguna de las líneas circundantes y mover se puede ver que el objeto hace rotación según el eje que se haya elegido.  Para rotar sin depender de ningún eje, es decir, libremente, se da clic dentro de las esferas circundantes, pero sin seleccionar ninguna.  Si se selecciona la línea global (en este caso la blanca) se rotaría dependiendo de la cámara o vista.
        
          .col-lg-7
            figure
              img(src='@/assets/curso/tema2/imagen7.png', alt='Botón rotar')
              figcaption Nota. Botón rotar.
        .row.justify-content-center.mt-4
          .col-lg-4.mb-4.mb-md-0
            h4 Botón escala
            p Se usa para hacer más grande o pequeño el objeto. Al dar clic sobre él y seleccionar un objeto se muestran nuevamente 3 líneas que representan los ejes, esta vez terminadas en cubo como se visualiza, a continuación:
          .col-lg-7
            figure
              img(src='@/assets/curso/tema2/imagen8.png', alt='Botón escala')
              figcaption Nota. Botón escala.
        .row.justify-content-center.mt-4
          .col-lg-4.mb-4.mb-md-0
            h4 Ejemplos botón escala
            p Dependiendo del eje seleccionado, y al estirarse al dar clic, el objeto escalará siguiendo esas coordenadas.  A continuación, se muestran algunos ejemplos:
        
          .col-lg-7
            figure
              img(src='@/assets/curso/tema2/imagen9.png', alt='Ejemplos botón escalar')
              figcaption Nota. Ejemplos botón escalar.
        .row.justify-content-center.mt-4
          .col-lg-4.mb-4.mb-md-0
            h4 Botón escala
            p Por otra parte, si se quiere escalar uniformemente se selecciona el cubo interior que aparece en el objeto como se muestra a continuación:
          .col-lg-7
            figure
              img(src='@/assets/curso/tema2/imagen10.png', alt='Ejemplos botón escalar')
              figcaption Nota. Ejemplos botón escalar.
    //- titulo con fondo
    .row.mb-5(data-aos="fade-down-right")
      .col-auto.fondo-3.px-4.py-2
        h2.mb-0.text-white Ventana Project
    p.mb-5(data-aos="fade-down-right") Esta ventana es la que contendrá los elementos del proyecto, su carpeta estará asociada a una carpeta en el computador.  A continuación, se encuentra una figura en la que se enumeran algunos de sus componentes:
    .row.justify-content-center.mb-5
      .col-lg-8.col-md-10.col-sm-12
        .titulo-sexto.color-acento-contenido.mb-4(data-aos="fade-down-right")
          p.mb-0 #[b Figura 5]
          p.mb-0 Ventana Project
        figure(data-aos="fade-down-right")
          img(src='@/assets/curso/tema2/imagen11.svg', alt='Ventana <em>Project</em>')
          figcaption Elementos ventana Project
    ol.lista-ol--cuadro.lista-ol--separador.mb-5
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span 1
        |  Permite crear una variedad de elementos para el proyecto.
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span 2
        |  En Assets se pueden agregar elementos y organizarlos por carpetas.  También se puede usar la sección de favoritos en la cual estarán los elementos más utilizados.
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span 3
        |  Se pueden ver los elementos disponibles, las carpetas, sonidos, modelos, entre otros.
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span 4
        |  Este #[i slider] permite aumentar o reducir el tamaño de los assets que se tienen en la sección del ítem 3.
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span 5
        |  Permite buscar elementos por su nombre. 
      li(data-aos="fade-down-right") 
        .lista-ol--cuadro__vineta
          span 6
        |  El candado bloquea la ventana, así no será posible su modificación. Con el símbolo de los 3 puntos se pueden agregar columnas u otro tipo de ventanas.
    //- titulo con fondo
    .row.mb-4(data-aos="fade-down-left")
      .col-auto.fondo-3.px-4.py-2
        h2.mb-0.text-white Ventana Scene View
    p.mb-5(data-aos="fade-down-left") En esta ventana se crean los escenarios y se posicionan los elementos que se requieren para su construcción, tales como cámaras, luces, entre otros. A continuación, se enumeran algunos de sus componentes:
    .titulo-sexto.color-acento-contenido.mb-4(data-aos="fade-down-right")
      p.mb-0 #[b Figura 6]
      p.mb-0 Ventana Scene View
    figure.mb-4(data-aos="fade-down-right")
      img(src='@/assets/curso/tema2/imagen11.svg', alt='Ventana <em>Scene View</em>')
      figcaption Elementos ventana Scene View.
    p(data-aos="fade-down-left") Los iconos de la sección navegación permiten desplazarse por la escena, y los de la sección transformación permiten rotar, mover  y escalar los objetos en la escena.
    p.mb-4(data-aos="fade-down-left") La pestaña Shaded permite modificar la manera en que se visualiza el escenario, se puede cambiar a una vista alambrada para observar los polígonos que componen los elementos, como se muestra a continuación:
    .titulo-sexto.color-acento-contenido.mb-4(data-aos="fade-down-right")
      p.mb-0 #[b Figura 7]
      p.mb-0 Shaded
    figure.mb-4(data-aos="fade-down-left")
      img(src='@/assets/curso/tema2/imagen12.svg', alt='<em>shaded</em>')
      figcaption Elementos ventana Shaded.
    p.mb-4(data-aos="fade-down-left") Con los botones señalados en la siguiente figura se puede activar o desactivar de la escena las luces, los sonidos y la ambientación.
    .titulo-sexto.color-acento-contenido.mb-4(data-aos="fade-down-right")
      p.mb-0 #[b Figura 8]
      p.mb-0 Botones de activación
    figure.mb-5(data-aos="fade-down-left")
      img(src='@/assets/curso/tema2/imagen13.svg', alt='<em>Shaded</em> - botones de activación')
      figcaption Elementos ventana Shaded - botones de activación.
    //- titulo con fondo
    .row.mb-4(data-aos="fade-down-right")
      .col-auto.fondo-3.px-4.py-2
        h2.mb-0.text-white Ventana Game View
    p.mb-4(data-aos="fade-down-right") Aquí se puede visualizar la compilación de los objetos y funciones del videojuego a través de la cámara que los esté observando.
    .titulo-sexto.color-acento-contenido.mb-4(data-aos="fade-down-right")
      p.mb-0 #[b Figura 9]
      p.mb-0 Game View
    figure.mb-5(data-aos="fade-down-left")
      img(src='@/assets/curso/tema2/imagen14.svg', alt='Elementos ventana <em>Game View</em>')
      figcaption Nota. Elementos ventana Game View.
    ul.lista-ul--color.lista-ul--separador.mb-5
      li(data-aos="fade-down-left")
        i.fas.fa-cube
        | #[b Display:] opciones de menú para escoger la vista de la cámara de la escena, por defecto está configurado Display 1.
      li(data-aos="fade-down-left")
        i.fas.fa-cube
        | #[b Free Aspect:]  valores predefinidos para probar cómo se vería el videojuego en distintos formatos.
      li(data-aos="fade-down-left")
        i.fas.fa-cube
        | #[b Scale:] permite hacer zoom en la ventana de juego para visualizar con mayor detalle el juego o para ver de manera global cómo se ve desde lejos.
      li(data-aos="fade-down-left")
        i.fas.fa-cube
        | #[b Maximize on Play:] si esta activa, al ejecutar el juego en modo Play la ventana Game se maximiza para jugar en pantalla completa.
      li(data-aos="fade-down-left")
        i.fas.fa-cube
        | #[b Mute Audio:] al activarla se silencia el audio del juego cuando está en modo Play.
      li(data-aos="fade-down-left")
        i.fas.fa-cube
        | #[b Status:] activa/inactiva la ventana de estadísticas, la cual muestra información del renderizado gráfico y audio al estar en modo Play.
      li(data-aos="fade-down-left")
        i.fas.fa-cube
        | #[b Gizmos:] activa/inactiva la visualización de cierto tipo de gizmos o iconos que se muestran en la venta escena.
    //- titulo con fondo
    .row.mb-4(data-aos="fade-down-right")
      .col-auto.fondo-3.px-4.py-2
        h2.mb-0.text-white Tipos de archivos
    .row.justify-content-center.mb-4
      .col-lg-5.col-md-12.mb-4.mb-lg-0(data-aos="fade-down-right")
        p.mb-4 A través de la ventana Project se crean las carpetas para organizar el proyecto como se muestra a continuación:
        .titulo-sexto.color-acento-contenido.mb-4(data-aos="fade-down-right")
          p.mb-0 #[b Figura 10]
          p.mb-0  Tipos de archivos
        .row
          .col-lg-10.col-md-12
            figure.mb-5(data-aos="fade-down-left")
              img(src='@/assets/curso/tema2/imagen15.svg', alt='Tipos de archivos')
              figcaption Nota. Elementos ventana tipos de archivos.     
      .col-lg-7.col-md-12(data-aos="fade-down-left")
        img(src='@/assets/curso/tema2/imagen16.jpg')
    AcordionA(tipo="a" clase-tarjeta="tarjeta tarjeta--gris")(data-aos="fade-down-right")
      .row.justify-content-around(titulo="Archivo tipo escena")
        .col-lg-11.mb-4.mb-lg-0
          p.mb-4 Se crea por defecto al abrir un proyecto nuevo y se ubica en la carpeta <em>scenes</em>.  Una escena es similar a un nivel del videojuego, esta contendrá elementos tales como cámaras, luces, personajes, acciones y comportamientos específicos en ella. Por ello, si se necesitan más escenas para crear por ejemplo nuevos niveles, la forma de hacerlo sería en el menú principal, <em>File - New Scene</em> o utilizando el comando control + N. Ver ejemplos en las siguientes figuras:

        .col-lg-5.mb-5
          figure
            img(src='@/assets/curso/tema2/imagen23.png')
            figcaption Nota. Elementos ventana <em>New Scene</em>.
        .col-lg-5.mb-5
          figure
            img(src='@/assets/curso/tema2/imagen18.png')
            figcaption Nota. Elementos ventana <em>New Scene</em> - clic derecho ventana inferior, <em>Create - Scene</em>.

      .row.justify-content-around(titulo="Archivo tipo material")
        .col-lg-11.mb-4.mb-lg-0
          p.mb-4 El material es la forma en que se van a ver los objetos, es decir, características como texturas, color, relieve, entre otros.  Lo primero que se hará es crear una carpeta para mantener organizados los elementos, esta carpeta se ubicará en la pestaña <em>assets</em> de proyecto, una vez creada (clic derecho Create - Folder) se da doble clic en ella. Las siguientes figuras muestran dichos ejemplos:

        .col-lg-5.mb-4.mb-lg-0
          figure
            img(src='@/assets/curso/tema2/imagen21.png')
            figcaption Nota. Elementos carpeta materiales.
        .col-lg-5.mb-4.mb-lg-0
          figure
            img(src='@/assets/curso/tema2/imagen24.png')
            figcaption Nota. Elementos ventana Create Material - clic derecho dentro de la carpeta, Create - Material.

        .col-lg-5.mb-4.mb-lg-0
          p.mb-4 Al ejecutar el paso descrito previamente aparecerá el material, y a la derecha en la pestaña inspector mostrará sus atributos o especificaciones, como puede verse en la siguiente figura:
          figure
            img(src='@/assets/curso/tema2/imagen19.png')
            figcaption Nota. Elementos ventana Inspector - Material.
        .col-lg-5
          p.mb-4 En este caso se selecciona <em>Shader - Standard</em> en la pestaña Inspector, se pueden cambiar características como por ejemplo el color una vez teniendo el material, en este caso un color simple sin más se procede a aplicarlo al objeto manteniendo presionado clic en el material y arrastrándolo encima del objeto, al hacerlo, este cambia tal como se muestra a continuación:
          figure
            img(src='@/assets/curso/tema2/imagen20.png')
            figcaption Nota. Ejemplo aplicación material a objeto.
            
      .row.justify-content-around(titulo="Archivo tipo <em>script</em>")
        .col-lg-5.mb-4.mb-lg-0
          p.mb-4 Son instrucciones de programación para que el objeto a quien se le asigna realice dichos comportamientos y funciones. La ruta de creación es en la pestaña <em>Proyecto - Create – C# Script</em>, como se muestra en la siguiente figura.
          figure
            img(src='@/assets/curso/tema2/imagen25.png')
            figcaption Nota. Crear C# <em>Script</em>.
        .col-lg-5.mb-4.mb-lg-0
          p.mb-4 La forma de aplicarlo al objeto es similar al material, es decir, se arrastra al objeto para verificar su aplicación y se puede hacer a través de la pestaña Inspector, seleccionando previamente el objeto al que se aplicó el <em>script</em>, tal como se puede ver en la siguiente figura.
          figure
            img(src='@/assets/curso/tema2/imagen26.png')
            figcaption Nota. Verificar aplicación C# <em>Script</em>.
            
      .row.justify-content-around(titulo="Tipos de archivos externos")
        .col-lg-5.mb-4.mb-lg-0
          p.mb-4 Unity tiene elementos 3D básicos, si se quiere utilizar elementos más desarrollados se deben crear en programas externos, y luego importarlos, en este caso se pueden importar los archivos. fbx simplemente arrastrándolos desde la carpeta del computador hacia la ventana proyecto, en una nueva carpeta creada para los personajes o modelados, como se muestra en la siguiente figura.
          figure
            img(src='@/assets/curso/tema2/imagen27.png')
            figcaption Nota. Visualización elementos externos agregados.
        .col-lg-5
          p.mb-4 También se puede importar archivos de texturas de la misma manera, es decir, arrastrándolos desde la carpeta del computador al proyecto, con esto se creará un nuevo material. Ver muestra en la siguiente figura:
          figure
            img(src='@/assets/curso/tema2/imagen28.png')
            figcaption Nota. Visualización texturas agregadas.
        .col-lg-5.mb-4.mb-lg-0
          p.my-4 En este caso se usa la textura tipo roca en formato de archivo .jpg, la cual se aplica al cubo. Si se quiere conservar el material azul, pero con textura rocosa como la imagen de muestra, la forma de aplicarlo es la siguiente: el material se arrastra de la pestaña proyecto hacia la casilla cuadrada al lado de la opción Albedo en la pestaña Inspector que está a la derecha, ver el ejemplo en la siguiente figura:
          figure
            img(src='@/assets/curso/tema2/imagen29.png')
            figcaption Nota. Ejemplo aplicación textura.
        .col-lg-5.mb-4
          p.mb-4 De la misma manera se agregan archivos en formato .mp3. wav. ogg. Para el caso del ejemplo se usará .mp3, la manera de integrarlo es idéntica, arrastrándolos desde la carpeta del computador al proyecto, como se muestra a continuación:
          figure
            img(src='@/assets/curso/tema2/imagen30.png')
            figcaption Nota. Ejemplo agregar archivos de audio.
        .col-lg-5
          p.mb-4 Una vez importado el archivo de audio se puede escuchar en el panel Inspector, en la parte inferior, dando clic en el botón Play, como se muestra en la siguiente figura.
          figure
            img(src='@/assets/curso/tema2/imagen31.png')
            figcaption Nota. Play archivo de audio.
        .col-lg-5

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
