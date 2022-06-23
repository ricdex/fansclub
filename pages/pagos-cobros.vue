<template>
  <section class="container">
    <div>
      <app-header :contentHeader="itemHeader" />
      <app-online />
      <app-programa />
      <app-carrousel :slider="itemsArray" />
      <app-help />
    </div>
  </section>
</template>

<script>
import AppHeader from '~/components/AppHeader.vue'
import AppCarrousel from '../components/AppCarrousel.vue'
import AppHelp from '../components/AppHelp'
import AppOnline from '../components/AppOnline.vue'
import AppPrograma from '../components/AppPrograma.vue'

let item = [
      {
        "icon": "assets/images/slider-1.png",
        "title": "Pago de Servicios",
        "paragraph": "Recarga tu celular y paga tus servicios sin salir de casa",
        "link": "/",
        "textlink": "Ver Pago de Servicios"
      },
      {
        "icon": "assets/images/slider-3.png",
        "title": "Préstamo",
        "paragraph": "Tu crédito fácil y rápido",
        "link": "/",
        "textlink": "Ver Préstamo"
      },
      {
        "icon": "assets/images/slider-2.png",
        "title": "Ahorro e inversión",
        "paragraph": "Invertir y disfrutar de tu ahorro nunca fue tan sencillo.",
        "link": "/",
        "textlink": "Ver ahorro e Inversión"
      },
      {
        "icon": "assets/images/slider-4.png",
        "title": "Seguro",
        "paragraph": "Hagas lo que hagas, pon tu seguridad adelante.",
        "link": "/",
        "textlink": "Ver Seguro"
      }
    ]


let itemHeaderArray= {
  image: 'assets/images/pagos.png',
  preTitle: 'EMPRESAS / MÉTODOS DE PAGO',
  title: 'Envia Recibe y Solicita Dinero',
  paragraph: 'Somos una plataforma que brinda servicios financieros 100% online.Cuando se trata de tus finanzas, crecemos juntos en tu plan de juego.',
  textButton: 'Crear cuenta para iniciar',
  linkButton: '/',
  textpreButton: '',
  linkpreButton: '/',
}



export default {
  components: {
    AppHeader,
    AppCarrousel,
    AppHelp,
    AppOnline,
    AppPrograma
  },
  data() {
   return {
    itemHeader: itemHeaderArray,
    itemsArray: item
   }
 }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Baloo+2&display=swap');
body {
  font-family: 'Baloo 2', cursive;
}
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>

