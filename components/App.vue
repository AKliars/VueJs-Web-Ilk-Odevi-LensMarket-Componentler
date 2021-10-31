<template>
  <div id="app">
      <ust-menu></ust-menu>
      <uye-girisi></uye-girisi>
      <filtreleme></filtreleme>
      <urun-detay></urun-detay>
      <side-bar></side-bar>
      <urunler></urunler>
      <yorumlar></yorumlar>
      <markalar></markalar>
      <sepet></sepet>
       <carousel>
            <carousel-slide v-for="slide in slides" :key="slide" class="carousel-slider">
                <img :src="slide" :alt="slide">
            </carousel-slide>
        </carousel>
      
  </div>
</template>

<script>
import ustMenu from "./components/ustMenu.vue"
import uyeGirisi from "./components/uyeGirisi.vue"
import sideBar from "./components/sideBar2.vue"
import filtreleme from "./components/filtreleme.vue"
import urunDetay from "./components/urunDetay.vue"
import urunler from "./components/urunler.vue"
import yorumlar from "./components/yorumlar.vue"
import markalar from "./components/markalar.vue"
import sepet from "./components/sepet.vue"
import Carousel from './components/Carousel.vue';
import CarouselSlide from './components/CarouselSlide';




export default {
  name: 'app',
  data(){
        return {
            slides: [
                'https://cdn.lensmarket.com/ext/banners/58659929202109201459.jpg',
                'https://cdn.lensmarket.com/ext/banners/7424077906202110011159.jpg',
                'https://cdn.lensmarket.com/ext/banners/4397766027202106281429.jpg',
                'https://cdn.lensmarket.com/ext/banners/2271106865202106191041.jpg',
                'https://cdn.lensmarket.com/ext/banners/8151521360202108191348.jpg',
                'https://cdn.lensmarket.com/ext/banners/4915161971202105231615.jpg',
                'https://cdn.lensmarket.com/ext/banners/e21bfee7e46a4ab2d4b2aac007dfcde5_banner-web.jpg',
            ]
        }
    },
  components : {
    ustMenu ,
    uyeGirisi,
    sideBar,
    filtreleme,
    urunDetay,
    urunler,
    yorumlar,
    markalar,
    sepet,
    Carousel,
    CarouselSlide
    }

}
</script>
<style>
.carousel {
        position:relative;
        overflow: hidden;
        width:90%;
        margin: 0 auto;
        height:500px;
        z-index:10;
    }
    .btn {
        padding:5px 10px;
        border:1px solid transparent;
        margin:5px 10px;
        color:#FFF;
        background: none;
        position:absolute;
        margin-top:-25px;
        z-index:2;
        font-size: 50px;
        font-weight: 100;
    }
    .btn:hover {
        cursor: pointer;
    }
    .btn:focus{
        outline:none;
    }
    .btn-next {
        top:50%;
        right:0;
    }
    .btn-prev {
        top:50%;
        left:0;
    }
    .carousel-slider {
        position:absolute;
        top:0;
        left:0;
        bottom:0;
        right:0;
    }
    .carousel-slider img {
        width:100%;
        height:100%;
    }
</style>