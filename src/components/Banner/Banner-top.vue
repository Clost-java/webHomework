
<script setup>
 import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';
import 'swiper/css/effect-cube';
import 'swiper/css/pagination';
import { EffectCube, Pagination } from 'swiper';
import { reactive } from '@vue/reactivity';


 let SwiperImages = reactive(["https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/6d90fda69e63bf93ae62120901bafc0e.jpg?thumb=1&w=2452&h=920&f=webp&q=90",
 "https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/dce8b00fb3b4ebecbcf72353bff8a030.jpg?thumb=1&w=2452&h=920&f=webp&q=90",
 "https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/454c1da2c5b64a3f2c07c5a4c01aa9c4.jpg?thumb=1&w=2452&h=920&f=webp&q=90",
 "https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/b836faf5402e8c14b626507b5c2e0ed5.jpeg?w=2452&h=920"]) 
let BannerBarData = reactive(["手机","电视","家电","笔记本 平板","出行 穿戴","耳机 音箱","健康 儿童","生活 箱包","智能 路由器","电源 配件"])


</script>

<template>
<div class="banner">
    <div class="container">
    <div class="swiper-container">
            <Swiper
    :effect="'fade'"
    :grabCursor="true"
    :loop="true"

    :pagination="true"
    :modules="[EffectCube, Pagination]"
  >
     <SwiperSlide v-for="(img,index) in SwiperImages" :key="index"><img :src="img" alt=""></SwiperSlide>
             <div class="bannerBar">
            <ul>
                <li v-for="(item,index) in BannerBarData" :key="index">
                <a href="#">{{item}}</a>
                <em class="right">&gt;</em>
                </li>
            </ul>
        </div>

  
  </Swiper>
    </div>


    </div>
    
</div>
  
</template>

<style scoped>
.container{
    width: 1280px;
    margin: 0 auto;
}
.swiper-container{
    position: relative;
}
.bannerBar{
    position: absolute;
    z-index: 10;
    top:10px;
    opacity: 0.5;
}
img{
    width: 100%;
}
.bannerBar li a{
    display: inline-block;
    height: 42px;
    width: 200px;
    line-height: 42px;
    box-sizing: border-box;
    font-size: 16px;
    color: #ffffff;
    padding-left:20px ;
}
.bannerBar li em{
    font-size: 16px;
    font-weight: bolder;
    color: #ffffff;
}


</style>