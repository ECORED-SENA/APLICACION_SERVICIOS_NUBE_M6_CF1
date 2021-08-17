<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal
      .titulo-principal__numero
        span 3
      h1 Introducción a la arquitectura orientada a servicios
    .row.mt-5
      .col-12.col-lg-7
        p Hasta el momento se han venido revisando las tecnologías para el desarrollo web, por lo que es necesario entender que aparte de crear aplicaciones también se pueden crear servicios. Para esto es necesario abordar de manera sucinta el concepto de la Arquitectura Orientada a Servicios llamada SOA. Al respecto es un tipo de arquitectura de software, la cual se basa en la integración de aplicaciones mediante servicios. Según IBM, se define SOA, como:
        .row.mb-5 
          .col-12
            .cajon.color-acento-contenido.px-5.py-4.mb-3
              p “…una manera de hacer que los componentes de software sean reutilizables a través de interfaces de servicio. Estas interfaces utilizan estándares de comunicación comunes entre sí, de tal manera que pueden incorporarse rápidamente a nuevas aplicaciones sin tener que realizar una integración profunda cada vez…”. #[strong (SOA, 2021)]
      .col-5.d-none.d-lg-block
        figure
          img(src="@/assets/template/tema-3-6.png" alt="Texto que describa la imagen")
    .row.mt-5
      .col-3.d-none.d-lg-block
        figure
          img(src="@/assets/template/tema-3-5.svg" alt="Texto que describa la imagen")
      .col-12.col-lg-9
        p En ese sentido, es interesante el desarrollo software en sí, la reutilización de componentes, y la comunicación con distintas aplicaciones sin tener la necesidad de crear un desarrollo a la medida para cada aplicación al cual se quiera conectar. Es por eso por lo que nace el concepto de servicio y de interoperabilidad.
        p.mt-3 Como una de las implementaciones de SOA existen las arquitecturas REST y SOAP, las dos siguen los mismos “principios” de SOA. Por tanto, REST y SOAP son dos vías distintas para la transmisión de datos en línea. Específicamente, ambas definen cómo diseñar interfaces de programación de aplicaciones (API), que no es más que una tecnología que sirve como un medio para que dos aplicaciones o plataformas se puedan comunicar entre sí y lo hacen exponiendo o publicando un conjunto de servicios y reglas para cómo acceder a ellos. La principal diferencia es que SOAP es un protocolo, y REST no lo es. Por lo general, alguno de ellos regirá a las API, es decir definirá una serie de reglas para la publicación de los servicios como también del acceso, según el caso práctico y las preferencias del desarrollador.
      
    #t_3_1.titulo-segundo.mt-5
      .h4 3.1 SOAP
    figure
      img(src="@/assets/template/tema-3-1.png" alt="Texto que describa la imagen")
    .row.mt-5
      .col-12.col-lg-9
        p Por sus siglas protocolo simple de acceso a objetos. Se define como un protocolo o reglas estándar que se creó principalmente para permitir la comunicación entre las aplicaciones que estaban desarrolladas con diferentes lenguajes y además que reposaban en distintas plataformas tecnológicas. Por tener la naturaleza de un protocolo, existen reglas integradas que aumentan la complejidad y la sobrecarga en los servidores, lo cual causa que pueda haber retrasos en el tiempo que tardan las páginas en cargarse o dar alguna respuesta. No obstante, estos estándares por su estructura y seguridad son más demandados en el sector empresarial. #[strong (RedHat, 2021)]
        p.mt-3 Adicionalmente, el envío de una solicitud de datos a una API de SOAP se puede administrar a través de cualquiera de los protocolos de la capa de la aplicación, por ejemplo, HTTP que es usado por los exploradores web, SMTP que es protocolo usado por los correos electrónicos, TCP, entre otros. No obstante, una vez que se recibe una solicitud, los mensajes SOAP de retorno devuelve por defecto documentos XML, que es un lenguaje de etiquetas que es comprensible tanto para las máquinas como para las personas.
      .col-3.d-none.d-lg-block
        figure
          img(src="@/assets/template/tema-3-2.svg" alt="Texto que describa la imagen")
    #t_3_2.titulo-segundo.mt-5
      .h4 3.2 REST
    figure
      img(src="@/assets/template/tema-3-3.png" alt="Texto que describa la imagen")
    p.mt-5 Por sus siglas en inglés, Representational State Transfer, traduce transferencia de estado representacional. Se define como un compendio de lineamientos que se ajustan a las necesidades de los servicios web y especialmente a las aplicaciones móviles por la velocidad de transmisión y por lo ligero de la información. Cuando se envía una solicitud de datos a una API de REST, se hace a través de un protocolo de transferencia de hipertexto, comúnmente denominado HTTP. Una vez que reciben la solicitud, las API diseñadas para REST (conocidas como API o servicios web de RESTful) dan como respuesta mensajes en diversos formatos como pueden ser HTML, XML, JSON, entre otros. El formato más usado para los mensajes es la notación de objetos JavaScript (JSON). Este formato puede leerlo cualquier lenguaje de programación, es liviano y es comprensible para las máquinas como para las personas. De esta forma, las API de RESTful son más flexibles y se pueden configurar con mayor facilidad. #[strong (RedHat, 2021).] 
    .row.mt-3 
      .col-10.offset-1
        .cajon.color-acento-contenido.px-5.py-4.mb-4
          .row
            .col-4.col-lg-3.offset-4.offset-lg-0.align-self-center
              figure
                img(src="@/assets/template/tema-3-4.svg" alt="Texto que describa la imagen").w-75
            .col-12.col-lg-9.mt-4.mt-lg-0.align-self-center  
              p Como conclusión se tiene una comparación de estas dos arquitecturas: las API de REST son livianas, así que son ideales para los escenarios tecnológicos más nuevos, como lo son el internet de las cosas (IoT), el desarrollo de aplicaciones móviles y la informática sin servidor. Los servicios web de SOAP ofrecen seguridad y cumplimiento de las operaciones que están asociadas a la dinámica operativa de una empresa, sin embargo, al tener la rigurosidad de abarcar tantas reglas puede ser también muy pesada la gestión de la información.




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

<style lang="sass" scoped></style>
