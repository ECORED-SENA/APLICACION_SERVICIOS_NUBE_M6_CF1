<template lang="pug">
.curso-main-container.introduccion
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
  
    .titulo-principal
      .titulo-principal__numero
        span
          i.fas.fa-info
      h1 Introducción
    
    figure
      .video
        iframe(width="560" height="315" src="https://www.youtube.com/embed/RHYdOwQdVQc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    .row.mt-5
      .col-12.col-lg-10
        p El desarrollo de las aplicaciones y sistemas web, han sido una tendencia desde las últimas tres décadas y sus mejoras han ido evolucionando conforme a las innovaciones de la infraestructura tecnológica que las soporta. Hoy en día vemos que las aplicaciones son mucho más interactivas, más rápidas, más seguras y usables, un ejemplo de esto es cuando se ingresa a un sitio web desde un dispositivo móvil, otro ejemplo es cuando vemos un video de YouTube, cuando conversamos por WhatsApp o vemos una serie en Netflix. Todas estas condiciones y aspectos se dan gracias a una robusta infraestructura de hardware que permite el despliegue no solo de aplicaciones sino de servicios que son usualmente utilizados día a día. En ese sentido, es importante comprender los primeros componentes que enriquecen y dan rigurosidad a la construcción de esta naturaleza de sistemas.  
        
      .col-4.col-lg-2.offset-4.offset-lg-0.align-self-center
        figure
            img(src="@/assets/template/tema-0-2.svg" alt="Texto que describa la imagen")



</template>

<script>
export default {
  name: 'Introduccion',
  data: () => ({
    // variables de vue
  }),
}
</script>

<style lang="sass" scoped>
.introduccion
</style>
