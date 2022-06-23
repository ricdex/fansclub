<template>
  <section class="container">
    <div>
      <app-header :contentHeader="itemHeader" />
      <div class="container-factura">
        <b-row>
            <b-col cols="4">
                <img src="~/assets/images/beneficio-1.png" alt="logo-fanclub" class="logo" style="height: 70px;" />
                <h5> <strong>¡En el ángulo!</strong></h5>
                <p>Ponemos a tu alcance una variedad de productos y servicios financieros a lamedida de tus necesidades de forma simple, rápida y segura. ⚽🙌 </p>
            </b-col>
            <b-col cols="4">
                <img src="~/assets/images/valor-4.png" alt="logo-fanclub" class="logo"  style="height: 70px;" />
                <h5> <strong>¡Somos hinchas, seámoslo siempre!</strong></h5>
                <p>Nos ponemos la camiseta beneficiando con comisiones de nuestros ingresos al equipo de tus amores. Al registrarte, ya sea como persona natural o empresa, sólo deberás indicar a qué club deseas beneficiar y listo! Directo a tu club, para que crezca como tú! 💰🏆</p>
            </b-col>
            <b-col cols="4">
                <img src="~/assets/images/ahorro.png" alt="logo-fanclub" class="logo" style="height: 70px;" />
                <h5> <strong>Costos Reducidos</strong></h5>
                <p>Te presentamos las mejores opciones, con costos super competitivos en cada uno de nuestros productos y servicios financieros. </p>
            </b-col>
        </b-row>
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
  image: 'assets/images/facturacion.png',
  preTitle: 'EMPRESAS',
  title: 'Facturación',
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
.container-factura{
  position: relative;
  top: 80px;
  height: 400px;
}
/* .container-factura img{
  height: 200px;
} */
</style>

