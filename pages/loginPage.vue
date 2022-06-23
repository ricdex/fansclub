<template>
  <section class="container">
    <div>
      <app-iniciarsesion/>
    </div>
  </section>
</template>

<script>
import AppIniciarsesion from '../components/AppIniciarsesion.vue'



export default {
  components: {
    AppIniciarsesion
},
  data() {
   return {
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

