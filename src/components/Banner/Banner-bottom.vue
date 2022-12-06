<script setup>
import { reactive } from "@vue/reactivity";

let images = reactive(["src/assets/images/bPhone1.jpg","src/assets/images/bPhone2.jpg","src/assets/images/bPhone3.jpg"])
let textData= reactive([
    {imgUrl:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/82abdba456e8caaea5848a0cddce03db.png",text:"保障服务"},
    {imgUrl:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/806f2dfb2d27978e33fe3815d3851fa3.png",text:"企业团购"},
    {imgUrl:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/eded6fa3b897a058163e2485532c4f10.png?w=48&h=48",text:"F码通道"},
    {imgUrl:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/43a3195efa6a3cc7662efed8e7abe8bf.png?w=48&h=48",text:"米粉卡"},
    {imgUrl:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/43a3195efa6a3cc7662efed8e7abe8bf.png?w=48&h=48",text:"以旧换新"},
    {imgUrl:"https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/43a3195efa6a3cc7662efed8e7abe8bf.png?w=48&h=48",text:"话费充值"}
])
</script>

<template>
<div class="bannerBottom">
    <div class="container">
        <div class="text left">
            <ul>
                <li class="left" v-for="(item,index) in textData" :key="index">
                    
                    <a href=""><img :src="item.imgUrl" alt="">{{item.text}}</a>
                </li>
            </ul>
        </div>
        <div class="imgBox left">
            <ul>
                <li class="left" v-for="(img,index) in images" :key="index"><img :src="img" alt=""></li>
            </ul>
        </div>
    </div>
</div>
  
</template>

<style scoped>
.container{
    width: 1280px;
    margin: 20px auto;
}
.text{
    width: 234px;
    height: 170px;
    background-color: #5f5750;
}
.text a{
    color: #ffffff;
    position: relative;
    text-align: center;
    box-sizing: border-box;
    font-size: 14px;

}
.text ul {
    margin-top: 25px;
}
.text a img{
    width: 24px;
    height: 24px;
    position: absolute;
    bottom: 20px;
    left:15px;
   
}
.text ul li {
    margin: 20px 10px;
}



.imgBox{
    height: 170px;
}
.imgBox ul li {
    margin-left: 10px;
}
.imgBox img{
    width: 316px;
}


</style>