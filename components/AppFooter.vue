<template>
  <div class="container-footer">
    <b-row>
        <b-col cols="4" >
            <div>
                <img src="~/assets/images/logo-2.png" alt="logo-fanclub" class="logo" height="50px"/>
                <ul class="redes-sociales">
                    <li><b-icon icon="facebook"></b-icon></li>
                    <li><b-icon icon="linkedin"></b-icon></li>
                    <li><b-icon icon="twitter"></b-icon></li>
                    <li><b-icon icon="instagram"></b-icon></li>
                </ul>
            </div>
            
        </b-col>
        <b-col cols="2" >
            <h5><strong>Para Personas</strong></h5>
            <ul>
                <li>Tarjeta</li>
                <li>Pagos de Servicios</li>
                <li>Tu Cuenta</li>
                <li>Préstamos</li>
                <li>Ahorro e Inversión</li>
                <li>Seguros</li>
                <li>Tipo de Cambio</li>
            </ul>
        </b-col>
        <b-col cols="2" >
            <h5><strong>Para Empresas</strong></h5>
            <ul>
                <li>Pagos y Cobros</li>
                <li>Préstamos</li>
                <li>Factoring</li>
                <li>Leasing</li>
                <li>Tipo de Cambio</li>
                <li>Inversiones</li>
                <li>Tu Cuenta</li>
            </ul>
        </b-col>
        <b-col cols="2" >
            <ul>
                <li>Nosotros</li>
                <li>Regístrate</li>
                <li>Ayuda y Contacto</li>
                <li>Blog</li>
                <li>Política de Privacidad</li>
                <li>Términos y Condiciones</li>
            </ul>
        </b-col>
        <b-col cols="2" >
            <h5><strong>Contacto</strong></h5>
            <ul>
                <li>info@fansclub.co</li>
                <li>T. 01 700 3301</li>
                <li>C. 963 896 793</li>
                <li>Lunes a Viernes:</li>
                <li>8:00 am - 8:00 pm</li>
                <li>Sábados:</li>
                <li>9:00 am - 8:00 pm</li>
                <li>Av. Dirección 457 Cercado de Lima of.101 Urb Cercado de Lima, Lima</li>
            </ul>
        </b-col>
    </b-row>
    <b-row>
        <b-col cols="6" >
            <div>
                <img src="~/assets/images/libro-reclamaciones.png" alt="libro de reclamaciones" width= "18%"/>
            </div>
        </b-col>
        <b-col cols="6" >
            <div class="container-chatbox">
                <img src="~/assets/images/chatbox.png" alt="chatbox" class="chatbox" width="40%"/>
            </div>
        </b-col>
    </b-row>
  </div>
</template>

<style>
.container-footer {
    background-color: #F5F5F5;
}
.container-footer .logo{
    width: 50%;
    height: 80px;
}
.container-footer .row {
    margin-right: 0px;
    margin-left: 0px;
    padding: 45px 0px;
}
.container-footer ul {
    padding: 0;
}
.container-footer ul > li {
    list-style:none;
}
.container-footer .redes-sociales{
    display: flex;
    padding-left: 8%;
}
.container-footer .redes-sociales li{
    padding: 10px
}
.container-footer .container-chatbox{
    display: flex;
    justify-content: end;
}
</style>

