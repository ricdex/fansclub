<template>
  <section class="container">
    <div>
      <app-header :contentHeader="itemHeader" />
      <div class="container-factura">
        <h1>¡Con nosotros aseguras el gol de tu inversión!</h1>
        <br>
         <img src="~/assets/images/img-inversion.png" alt="logo-fanclub" class="logo" />
      </div>
      <app-carrousel :slider="itemsArray" />
      <app-help />
    </div>
  </section>
</template>

<script>
import AppHeader from '~/components/AppHeader.vue'
import AppCarrousel from '../components/AppCarrousel.vue'
import AppHelp from '../components/AppHelp'

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
  image: 'assets/images/foto-headerInversion.png',
  preTitle: 'EMPRESAS',
  title: 'Inversiones',
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
    AppHelp
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
.container-register {
    margin-top: 50%;
}
.container-factura{
  position: relative;
  top: 80px;
  height: 400px;
}
.container-factura img{
  height: 200px;
}
</style>

