<template>
  <div>
    <b-navbar toggleable="lg" type="dark">
      <b-navbar-brand href="/"> <img src="~/assets/images/logo.png" alt="logo-fanclub" height="50px"></b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="navbar-nav-first">
          <b-nav-item-dropdown text="Personas">
            <b-dropdown-item href="/proximamente">Tarjeta</b-dropdown-item>
            <b-dropdown-item href="/pagos-servicios">Pagos de Servicios</b-dropdown-item>
            <b-dropdown-item href="/proximamente">Préstamos</b-dropdown-item>
            <b-dropdown-item href="/inversion">Ahorro e inversión</b-dropdown-item>
            <b-dropdown-item href="/proximamente">Seguros</b-dropdown-item>
          </b-nav-item-dropdown>

          <b-nav-item-dropdown >
            <!-- Using 'button-content' slot -->
            <template #button-content>
              <span>Empresas</span>
              
            </template>
            <b-dropdown-item href="/pagos-cobros">Pagos y Cobros</b-dropdown-item>
            <b-dropdown-item href="/proximamente">Préstamos</b-dropdown-item>
            <b-dropdown-item href="/facturacion">Factoring</b-dropdown-item>
            <b-dropdown-item href="/proximamente">Leasing</b-dropdown-item>
            <b-dropdown-item href="/proximamente">Tipo de Cambio</b-dropdown-item>
            <b-dropdown-item href="/inversion-empresa">Inversiones</b-dropdown-item>
          </b-nav-item-dropdown>
          
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item href="#" class ="mx-2 link" right>Nosotros</b-nav-item>
          <b-nav-item href="#" class ="mx-2 link" right>Ayuda y Contacto</b-nav-item>
          <b-nav-item href="#" class ="mx-2 link" right>Blog</b-nav-item>

          <b-nav-form>
            <b-button size="sm" class="my-2 mx-2 my-sm-0" variant="outline-primary"> <a href="/iniciar-sesion"> Iniciar Sesión</a></b-button>
            <b-button size="sm" class="my-2 mx-2 my-sm-0 btn-registrate" > <a href="/registerPage">Registrate</a> </b-button>
          </b-nav-form>

        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>


<style>
  * {
    /* outline: 1px solid red; */
  }
  .navbar {
    background-image: url("~/assets/images/rectangulo.png");
    background-repeat: no-repeat, repeat;
    padding: none !important;
  }
  .navbar-nav-first span{
    color: white;
  }
  .navbar-nav-first .dropdown-toggle::after {
    color: #00E37A;
  }
  .navbar-nav .link .nav-link, .navbar-nav .link .nav-link:hover {
    color: #1A1C17;
  }
  .btn-outline-primary {
    border-color: #7A32FF !important;
    color: #7A32FF !important;
    border-radius: 80px;
    padding-left: 0 15px;
    font-size: 1rem;
   
  }
  .btn-outline-primary:hover {
    color: #fff !important;
    background-color: #7A32FF !important;
    border-color: #7A32FF !important;
}

  button.btn-registrate {
    background-color: #7A32FF;
    border-radius: 80px;
    padding-left: 0 15px;
    font-size: 1rem;
  }
</style>

