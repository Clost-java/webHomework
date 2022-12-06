<script setup>
import { reactive } from "@vue/reactivity";


let topbarData = reactive(
   ["小米官网","小米商城","MIUI","loT","云服务","天星数科","有品","小爱开放平台","企业团购","资质证照","协议规则","下载app","Select Location"],
  
)

</script>

<template>
<div class="topbar">
    <div class="container">
        <div class="topbar-left  left">
            <a href="#" v-for="(item,index) in topbarData" :key="index">{{item}}<span v-if="index!=12">|</span></a>
        </div>
        <div class="topbar-right  right">
            <a href="#">登录<span>|</span></a>
            <a href="#">注册<span>|</span></a>
            <a href="#">消息通知</a>
            <div class="buy">
                <img src="src\assets\images\buy.png" alt="">
                <a href=""> 购物车 (0)</a>
            </div>

        </div>
    </div>
</div>

  
</template>


<style scoped>
a{
    font-size: 12px;
    line-height: 40px;
    color: #b0b0b0;
}
span{
    margin: 0 6px;
    color: #424242;
}
.topbar{
    background-color: #333;
}
.container{
    height: 40px;
    width: 1280px;
    margin: 0 auto; 
}
.buy{
    width: 120px;
    box-sizing: border-box;
    display: inline-block;
    margin-left: 10px;
    padding-left: 15px;
    background-color: #424242;
}

</style>