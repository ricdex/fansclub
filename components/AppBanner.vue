<template>
  <div class="banner-container">
    <p>Ponemos a nuestro equipo de asesores financieros a tu disposición.</p>
    <b-button size="sm" class="mb-2 btn-whatsapp">
      <b-icon icon="whatsapp" aria-hidden="true" class="icon-whatsapp"></b-icon> Hablemos
    </b-button>
    <img src="~/assets/images/banner-text.png" alt="logo-fanclub" class="logo" width="100%" />
  </div>
</template>

<style>
    .banner-container {
        background-image: url("~/assets/images/banner.png");
        background-position: center; /* Center the image */
        background-repeat: no-repeat; /* Do not repeat the image */
        background-size: cover; /* Resize the background image to cover the entire container */
    }
    .btn-whatsapp, .btn-whatsapp:hover{
       background: #00E37A;
       border-radius: 15px;
       width: 15%;
    }
</style>
