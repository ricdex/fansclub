<template>
    <div class="container-help">
        <b-row style="height: 200px;">
            <b-col cols="6"  class="colFirst">
                <div>
                    <h5> <strong> Estamos para ayudarte </strong> </h5>
                    <p>Ponemos a nuestro equipo de asesores financieros a tu disposición.</p>
                </div>
                
            </b-col>
            <b-col cols="6"  class="colSecond">
                <b-button size="sm" class="mb-2 btn-whatsapp">
                    <b-icon icon="whatsapp" aria-hidden="true" class="icon-whatsapp"></b-icon> Hablemos
                </b-button>
            </b-col>
        </b-row>
    </div>
</template>

<style>
.container-help {
    background-color: #F5F5F5;
}
.btn-whatsapp, .btn-whatsapp:hover{
    background: #6F04E0;
    border-radius: 20px;
    width: 35%;
}
.container-help .colFirst {
    text-align: left;
    padding: 15px 50px;
}
.container-help .colFirst {
    display: inline-flex;
    align-items: center;
}
.container-help .colSecond{
    display: inline-flex;
    align-items: center;
    justify-content: center;
}
</style>