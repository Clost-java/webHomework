<script setup>
import { reactive } from '@vue/reactivity'
import Right from './BaseRight.vue'
import Left from './BaseLeft.vue'
const images = reactive({
    left:{url:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/059f14c9ba134897be7db7a7286f1bb5.jpg?thumb=1&w=468&h=1228&f=webp&q=90"},
    right:{
        BigPic:[
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/nr-pub/202210262033_ef39fca0e37395d07682124770fd3ad9.png?thumb=1&w=400&h=400&f=webp&q=90",title:"Redmi Note 12 5G",descripe:"三星 OLED 护眼屏｜骁龙 5G 芯｜5000mAh 电量",price:"1199"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/nr-pub/202210262012_94dd4ca657adcebec0d11ea09dac8a03.png?thumb=1&w=400&h=400&f=webp&q=90",title:"Redmi Note 12 Pro",descripe:" IMX766 防抖相机｜OLED 柔性直屏｜67W 闪充",price:"1699"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/nr-pub/202210262024_83bfd34bb3f733d69d342acaf34aea58.png?thumb=1&w=400&h=400&f=webp&q=90",title:"Redmi Note 12 Pro+",descripe:"2亿超清防抖相机｜OLED 柔性直屏",price:"2199"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/50da95e9e4496dcac8704da2deb94f6e.jpg?thumb=1&w=400&h=400&f=webp&q=90",title:"Redmi Note 11 5G",descripe:"5000mAh大电量",price:"1099"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/28c14106b688ac7ae88e761564789b37.jpg?thumb=1&w=400&h=400&f=webp&q=90",title:"Redmi K50",descripe:"2K直屏的狠旗舰",price:"2099"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/5713971c4bb6512743dfd06023080268.png?thumb=1&w=400&h=400&f=webp&q=90",title:"Redmi Note 11T Pro",descripe:"天玑8100｜真旗舰芯",price:"1569"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/nr-pub/202207012000_0b9df066c110f201154013ac373df1d9.png?thumb=1&w=400&h=400&f=webp&q=90",title:"Xiaomi 12S Pro",descripe:"骁龙8+ 旗舰处理器 | 徕卡影像",price:"4399"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/nr-pub/202208101511_488638d8f8d5dbcf3b66cd82703ecfb9.png?thumb=1&w=400&h=400&f=webp&q=90",title:"Redmi K50 至尊版",descripe:"骁龙8+ ｜1.5K 高清直屏",price:"2799"}
]
    }
})



</script>


<template>

<div class="content">
  <div class="container">
      <div class="title">
          <h2 class="left">手机</h2>
          <a href="" class="right"><h2>查看更多</h2></a>
      </div>
      <Left :images="images.left"/>
      <Right :images="images.right"
                :hasSmallPic="false" />
  </div>
</div>
</template>



<style scoped>
.content{
  background-color: #F5F5F5;
}

.container{
  width: 1280px;
  height: 700px;
  margin: 0 auto;
}
.title{
    height: 80px;
}
.title h2{
    font-size: 22px;
    font-weight: 300;
    line-height: 80px;
    color: #333333;;
}



</style>