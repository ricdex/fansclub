<template>
  <section class="container">
    <div>
      <app-header :contentHeader="itemHeader" />
      <app-carrousel :slider="itemsArray" />
      <app-register-footer />
    </div>
  </section>
</template>

<script>
import AppHeader from '~/components/AppHeader.vue'
import AppCarrousel from '../components/AppCarrousel.vue'
import AppHelp from '../components/AppHelp'
import AppOnline from '../components/AppOnline.vue'
import AppPrograma from '../components/AppPrograma.vue'
import AppRegisterFooter from '../components/AppRegisterFooter'

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
  image: 'assets/images/proximamente.png',
  preTitle: '¡PRONTO!',
  title: 'Más beneficios y seguridad para tu inversión',
  paragraph: '',
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
    AppPrograma,
    AppRegisterFooter
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

