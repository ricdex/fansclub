<template>
  <section class="container">
    <div>
      <app-header :contentHeader="itemHeader" />
      <app-carrousel :slider="itemsArray" />
      <app-beneficio/>
      <app-banner/>
      <app-nosotros/>
      <div style="padding-top: 60px;">
        <img src="~/assets/images/filosofia.png" alt="logo-fanclub" class="logo" width="100%" />
      </div>
      <app-valores/>

    </div>
  </section>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'
import AppHeader from '~/components/AppHeader.vue'
import AppCarrousel from '../components/AppCarrousel.vue'
import AppBeneficio from '../components/AppBeneficio.vue'
import AppNosotros from '../components/AppNosotros.vue'
import AppBanner from '../components/AppBanner.vue'
import AppValores from '../components/AppValores.vue'

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
  image: 'assets/images/foto-header.png',
  preTitle: '',
  title: 'Haz un gol de media cancha en tus finanzas.',
  paragraph: 'Somos una plataforma que brinda servicios financieros 100% online.Cuando se trata de tus finanzas, crecemos juntos en tu plan de juego.',
  textButton: 'Crear cuenta para iniciar',
  linkButton: '/',
  textpreButton: 'Ver servicios para empresas',
  linkpreButton: '/',
}

// let itemHeader = {
//       preTile: 'personas',
//        title: 'Inversiones',
//        paragraph: 'Somos una plataforma que brinda servicios financieros 100% online.Cuando se trata de tus finanzas, crecemos juntos en tu plan de juego.',
//        textButton: 'Crear cuenta para iniciar',
//        linkButton: '/',
//        textpreButton: 'Ver servicios para empresas',
//        linkpreButton: '/',
//     }

// let usern = {
//        username: 'matt'
//     }

let itemsSlider = [1, 2, 3, 4];

export default {
  components: {
    AppLogo,
    AppHeader,
    AppCarrousel,
    AppBeneficio,
    AppNosotros,
    AppBanner,
    AppValores
  },
  data() {
   return {
      // itemsSlider : [1, 2, 3, 4]
    //  items: {
    //    username: 'matt'
    //  }
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

