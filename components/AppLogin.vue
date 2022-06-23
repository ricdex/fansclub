<template>
  <div class="container-login">
    <b-row>
        <b-col cols="6" >
            <div>
                <p>jfhsjdhfjdhsfjhdsf</p>

            </div>
        </b-col>
        <b-col cols="6" >
            <div class="form-login">
                <h2 style="color: #7A32FF;">Inicia Sesión </h2>
                <form @submit.prevent="handleSubmit">
                    <div class="form-group">
                        <label for="username">User</label>
                        <input type="text" v-model="username" name="username" class="form-control" :class="{ 'is-invalid': submitted && !username }" />
                        <div v-show="submitted && !username" class="invalid-feedback">Username is required</div>
                    </div>
                    <div class="form-group">
                        <label htmlFor="password">Contraseña</label>
                        <input type="password" v-model="password" name="password" class="form-control" :class="{ 'is-invalid': submitted && !password }" />
                        <div v-show="submitted && !password" class="invalid-feedback">Password is required</div>
                    </div>
                    <div>
                        <b-row>
                            <b-col cols="6">
                                <b-form-group v-slot="{ ariaDescribedby }">
                                    <b-form-radio  :aria-describedby="ariaDescribedby" name="some-radios" value="A">Recuérdame</b-form-radio>
                                </b-form-group>
                            </b-col>
                            <b-col cols="6"> <span>Mostrar contraseña</span></b-col>
                        </b-row>
                    </div>
                    <div class="form-group btn-container">
                        <button class="btn btn-primary btn-login btn-registrate" >Iniciar Sesion</button> <br>
                        <a href="">no recuerdas tu contraseña?</a>
                    </div>
                </form>
            </div>

            <div class="register-container">
                <b-row>
                    <b-col cols="6">
                        <span>¿Nuevo en FactorFC?</span>
                    </b-col>
                    <b-col cols="6" style="text-align: end;" > <b-button size="sm" class="my-2 mx-2 my-sm-0" >Crear una Cuenta</b-button> </b-col>
                </b-row>
            </div>
        </b-col>
    </b-row>
  </div>
</template>


<!-- <template>
  <div class="login-container">
    <b-row> -->
        <!-- <b-col cols="6" class="left-container">
            <div>
                <h5 style="color: #00E37A;"> <strong> Registro </strong> </h5>
                <h1>Inicia Sessión.</h1>
                <p>Únete a los más de 400.000 usuarios.</p>
                <b-button size="sm" class="my-2 mx-2 my-sm-0 btn-registrate" >Crear cuenta para iniciar</b-button>
            </div>
        </b-col> -->
        <!-- <b-col cols="6"> -->
            <!-- <div class="form-login">
                <h2 style="color: #7A32FF;">Inicia Sesión </h2>
                <form @submit.prevent="handleSubmit">
                    <div class="form-group">
                        <label for="username">User</label>
                        <input type="text" v-model="username" name="username" class="form-control" :class="{ 'is-invalid': submitted && !username }" />
                        <div v-show="submitted && !username" class="invalid-feedback">Username is required</div>
                    </div>
                    <div class="form-group">
                        <label htmlFor="password">Contraseña</label>
                        <input type="password" v-model="password" name="password" class="form-control" :class="{ 'is-invalid': submitted && !password }" />
                        <div v-show="submitted && !password" class="invalid-feedback">Password is required</div>
                    </div>
                    <div>
                        <b-row>
                            <b-col cols="6">
                                <b-form-group v-slot="{ ariaDescribedby }">
                                    <b-form-radio  :aria-describedby="ariaDescribedby" name="some-radios" value="A">Recuérdame</b-form-radio>
                                </b-form-group>
                            </b-col>
                            <b-col cols="6"> <span>Mostrar contraseña</span></b-col>
                        </b-row>
                    </div>
                    <div class="form-group btn-container">
                        <button class="btn btn-primary btn-login btn-registrate" >Iniciar Sesion</button> <br>
                        <a href="">no recuerdas tu contraseña?</a>
                    </div>
                </form>
            </div>

            <div class="register-container">
                <b-row>
                    <b-col cols="6">
                        <span>¿Nuevo en FactorFC?</span>
                    </b-col>
                    <b-col cols="6" style="text-align: end;" > <b-button size="sm" class="my-2 mx-2 my-sm-0" >Crear una Cuenta</b-button> </b-col>
                </b-row>
            </div> -->

        <!-- </b-col> -->
    <!-- </b-row>
  </div>
</template> -->

<style>
 .login-container {
}
.left-container{
    display: flex;
    align-items: center;
    text-align: left;
}
.register-container {
    background: #32E38A;
    padding: 10px;
    margin: 20px;
    border-radius: 10px;
    text-align: left;
    color: white;
}
.register-container .btn{
    background: #000000;
    border-radius: 15px;
}
.form-login{
    background: white;
    padding: 30px;
    margin: 20px;
    border-radius: 10px;
    text-align: left;
}
.form-login input{
    background: #CACACA;
    opacity: 0.2;
}
.form-login .btn-login, .form-login .btn-login:hover{
    background: #7C2EFE;
}
.form-login .btn-container{
    text-align: center;
}
.form-login a{
   color:  #7C2EFE
}
</style>

<script>
export default {
  data () {
        return {
            username: '',
            password: '',
            submitted: false
        }
    },
    computed: {
        // https://stackblitz.com/edit/vue-vuex-registration-login-example?file=login%2FLoginPage.js
        // ...mapState('account', ['status'])
        
    },
    created () {
        // reset login status
        // this.logout();
    },
    methods: {
        // ...mapActions('account', ['login', 'logout']),
        handleSubmit (e) {
            this.submitted = true;
            const { username, password } = this;
            if (username && password) {
                this.login({ username, password })
            }
        }
    }
};

</script>