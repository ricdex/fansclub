<template>
    <div class="container-register">
        <b-row>
            <b-col cols="6"  class="colFirst">
                <h1 class="container-h1">Abre una cuenta FansClub en unos minutos.</h1>
                <p>Únete a los más de 400.000 usuarios.</p>
                <b-button size="sm" class="my-2 mx-2 my-sm-0 btn-registrate" >Crea cuenta para iniciar</b-button>
            </b-col>
            <b-col cols="6" >
                <img src="~/assets/images/phone.png" alt="logo-fanclub" class="logo" width="100%" height="100%" />
            </b-col>
        </b-row>
    </div>
</template>

<style>
.container-h1 {
    font-weight: bold;
}
.container-register {
    background-color: #F5F5F5;
    max-height: 250px;
}
.container-register .colFirst{
    padding: 35px;
    text-align: left;
}
.container-register img {
    height: 75%;
    position: relative;
    top: -15%;
}
</style>