<script setup>
import { reactive } from '@vue/reactivity'
import Right from './BaseRight.vue'
import Left from './BaseLeft.vue'
const images = reactive({
    left:{url:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/06d75467973ea188caa56e18a67647b4.png?thumb=1&w=468&h=1228&f=webp&q=90"},
    right:{
        BigPic:[
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/f0408c24b677c7fe8b3cc402ec062334.png?thumb=1&w=400&h=400&f=webp&q=90",title:"Redmi G Pro 游戏本",descripe:"狂风调校的高能电竞本",price:"8999"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/0f8abb2bc3947c4679e3f1b2aafc28c0.jpg?thumb=1&w=400&h=400&f=webp&q=90",title:"Redmi Book Pro 15 2022",descripe:"全新12代英特尔处理器",price:"5599"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/e3c300330221ad788569e4fb1e6f932f.jpg?thumb=1&w=400&h=400&f=webp&q=90",title:"Redmi Book Pro 14 2022",descripe:"全新12代英特尔处理器，2.5K 120Hz高清屏，可选MX550独立显卡,CNC一体精雕工艺",price:"5399"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/b60f8c50789c123c11e060e7b283a315.jpg?thumb=1&w=400&h=400&f=webp&q=90",title:"RedmiBook Pro 15 R5/16G/512G 灰",descripe:"3.2K 超清视网膜全面屏 | 微米级一体精雕工艺	",price:"4499"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/01d9571051a91e540e5c644fa60cc858.jpg?thumb=1&w=400&h=400&f=webp&q=90",title:"Pro 14 增强版 i5 独显 - Win11",descripe:"2.5K超视网膜全面屏",price:"4799"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/nr-pub/202210261040_b679a0f353b618fc79a8b7ea930a19a1.png?thumb=1&w=400&h=400&f=webp&q=90",title:"Redmi Pad",descripe:"入门平板，屏幕/外观/系统三大升级",price:"1299"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/ed0541d2337dc4fff6e52c2b7f162fe5.jpg?thumb=1&w=400&h=400&f=webp&q=90",title:"小米平板5 Pro",descripe:"骁龙870芯片 | 2.5K超高清｜120HZ高刷新率 ",price:"2499"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/nr-pub/202208101511_488638d8f8d5dbcf3b66cd82703ecfb9.png?thumb=1&w=400&h=400&f=webp&q=90",title:"Redmi K50 至尊版",descripe:"骁龙8+ ｜1.5K 高清直屏",price:"549"}
],
    smallPic:{url:"https://cdn.cnbj1.fds.api.mi-img.com/nr-pub/202208101822_61eaf5f69fdc3e6c2fa0eb570e091d4d.png?thumb=1&w=200&h=200&f=webp&q=90",descripe:"小米平板5 Pro 12.4",price:"2999"}
    }
})



</script>


<template>

<div class="content">
  <div class="container">
      <div class="title">
          <h2 class="left">笔记本 | 平板</h2>
          <a href="" class="right">热门</a>
      </div>
      <Left :images="images.left"/>
      <Right :images="images.right"
                    :hasSmallPic="true"/>
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
.title a{
    font-size: 16px;
    line-height: 80px;
    margin-left: 5px;
    color: #333333;
}



</style>