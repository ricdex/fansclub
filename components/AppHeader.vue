<template>
  <div class="container-header">
    <b-row>
        <b-col cols="6"  class="col-first">
            <h5 style="color: #00E37A;"> <strong>{{contentHeader.preTitle}}</strong> </h5>
            <h1 style="font-weight: bold;">{{contentHeader.title}}</h1>
            <p>{{contentHeader.paragraph}}</p>
            <b-button size="sm" class="my-2 mx-2 my-sm-0 btn-registrate" >{{contentHeader.textButton}}</b-button>
            <a href="" style="color: #00E37A;font-weight: bold;">{{contentHeader.textpreButton}}</a>
        </b-col>
        <b-col cols="6" >
            <img :src="require(`@/${contentHeader.image}`)" alt="logo-fanclub" class="logo" width="100%"/>
        </b-col>
    </b-row>
  </div>
</template>

<style>
.container-header {
    position: relative;
    top: 50px;
}
.container-header .col-first {
    padding-top: 50px;
    text-align: left;
}
</style>

<script>

export default {
    props: ['contentHeader']
}

</script>



