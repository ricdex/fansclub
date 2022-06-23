<template>
    <div class="container-carousel">
        <div>
            <h4 style="text-align: left;"> Productos digitales para ti </h4> <br/>

            <!-- <p>sjfhsdfh {{ slider }}</p> -->

            <VueSlickCarousel ref="c1" :asNavFor="$refs.c2" :focusOnSelect="true" v-bind="settings">
                <div v-for="(item, index) in slider" :key="index">
                    <div class="item-container">
                        <!-- <img src="~/assets/images/slider-1.png" alt="slider-fanclub" class="slider" /> -->
                        <img :src="require(`@/${item.icon}`)" class="slider" alt="slider-fanclub" />
                        
                        <!-- <h1>{{item.icon}} </h1>
                        <h1>{{item.icon}}</h1> -->
                        <h4> <strong>{{item.title}}</strong> </h4>
                        <p>{{item.paragraph}}</p>
                        <a href="">{{item.textlink}} <b-icon icon="arrow-right" aria-hidden="true"></b-icon> </a>
                    </div>
                    <!-- <h1>{{item}}</h1> -->
                </div>
            </VueSlickCarousel>
        </div>
    </div>
</template>

<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";

var items = [1, 2, 3, 4,5,6,7];


export default {
// props: ['itemsSlider'],
  props: ['slider'],
  data: () => ({
    // items: itemsSlider,
    items: items,
    settings: {
        "dots": false,
        "slidesToShow": 3,
        "slidesToScroll": 1
    }
  }),
  components: {
    VueSlickCarousel
  }
};
</script>

<style>
.container-carousel {
    max-width: 1140px !important;
}
.container-carousel .item-container{
    padding: 35px 20px 20px;
    margin: 20px 5px;
    border: 1px solid #C4C4C4;
    box-shadow: 8px 4px 12px -2px rgb(0 0 0 / 20%);
    text-align: left;
    min-height: 260px;
}
.container-carousel .item-container img{
    margin-bottom: 10px;
}
.container-carousel .item-container a{
    color: #6F04E0 !important;
}
.slick-arrow {
    display: none !important;
}
</style>