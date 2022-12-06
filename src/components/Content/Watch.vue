<script setup>
import { reactive } from '@vue/reactivity'
import Right from './BaseRight.vue'
import Left from './BaseLeft.vue'
const images = reactive({
    left:{url:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/9895c56a7b792fb9053e3085fc261072.jpg?thumb=1&w=468&h=1228&f=webp&q=90"},
    right:{
        BigPic:[
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/nr-pub/202207011906_e7f02b803d3da16ec56a611e790243ba.png?thumb=1&w=400&h=400&f=webp&q=90",title:"小米手环7 Pro",descripe:"全彩方形大屏 | 独立GPS定位 | 多重健康监测",price:"369"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/nr-pub/202205240036_9a8fbf274c0d419c5a0a49ef67cdd7c8.png?thumb=1&w=400&h=400&f=webp&q=90",title:"小米手环7",descripe:"1.62″AMOLED 跑道屏 | 四大专业运动数据分析 | 活力竞赛·好友PK",price:"219"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/nr-pub/202205240036_9a8fbf274c0d419c5a0a49ef67cdd7c8.png?thumb=1&w=400&h=400&f=webp&q=90",title:"小米手环7 NFC版",descripe:"1.62″AMOLED 跑道屏 | 四大专业运动数据分析 | 活力竞赛·好友PK",price:"259"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/nr-pub/202204211419_626e47d8843927a9b719b9360d2b78dd.png?thumb=1&w=400&h=400&f=webp&q=90",title:"Xiaomi Watch Color 2",descripe:"60Hz高刷高清视网膜屏 | 心率监测 | 双频GPS四模定位",price:"699"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/f84503dbf5adbdf17111c61d4a7cf893.jpg?thumb=1&w=400&h=400&f=webp&q=90",title:"Redmi 手表2",descripe:"1.6AMOLED大屏 | 117种运动模式 | 24小时心率监测",price:"359"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/nr-pub/202204211417_27356c02de718e88afd3cf36eaba8097.png?thumb=1&w=400&h=400&f=webp&q=90",title:"Xiaomi Watch S1",descripe:"蓝宝石玻璃镜面 | 不锈钢中框 | 1.43”AMOLED大屏幕",price:"899"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/bf07c016f19ed9668024697c2396631e.jpg?thumb=1&w=400&h=400&f=webp&q=90",title:"小米手表Color 运动版",descripe:"超长续航，支持血氧功能",price:"549"},
    {url:"https://cdn.cnbj1.fds.api.mi-img.com/nr-pub/202208101511_488638d8f8d5dbcf3b66cd82703ecfb9.png?thumb=1&w=400&h=400&f=webp&q=90",title:"Redmi K50 至尊版",descripe:"骁龙8+ ｜1.5K 高清直屏",price:"549"}
],
    smallPic:{url:"https://cdn.cnbj1.fds.api.mi-img.com/nr-pub/202210191430_3ad0e4809ce06a126dea9755adbb2a1b.png?thumb=1&w=200&h=200&f=webp&q=90",descripe:"Xiaomi骨传导耳机",price:"699"}
    }
})



</script>


<template>

<div class="content">
  <div class="container">
      <div class="title">
          <h2 class="left">智能穿戴</h2>
          <a href="" class="right">穿戴</a>
          <a href="" class="right">耳机</a>
          
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