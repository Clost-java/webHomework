<script setup>
import { reactive } from "@vue/reactivity";

let navData = reactive(["Xiaomi手机","Redmi手机","电视","笔记本","平板","家电","路由器","服务中心","社区"])
let searchData = reactive(["全部商品","手机","加湿器","电视","小米平板5","红米","冰箱","显示器","笔记本"])

</script>

<template>
<div class="nav">
    <div class="container">
        <div class="logo">
            <img src="src\assets\images\logo-mi.png" alt="">
        </div>
        <ul>
            <li v-for="(item,index) in navData" :key="index"><a href="">{{item}}</a></li>
        </ul>

        <div class="search right">
            <input type="text" placeholder="小米">
            <button><img src="src\assets\images\search.png" alt=""></button>
        </div>
    </div>
</div>
</template>



<style scoped>

.container{
    height: 100px;
    width: 1280px;
    margin: 0 auto;
    position: relative;
}
.logo {
    position: absolute;
    width: 56px;
    height: 56px;
    top: 20px;
}

ul{
    position: absolute;
    left: 200px;
}
ul li{
    float: left;
    margin-left: 20px;
}
ul li a{
        line-height: 100px;
        color: #333333;
        font-size:16px ;
}
ul li a:hover{
    color: orange;
}

.search{
    position: relative;
}
.search input{
    width: 245px;
    height: 50px;
    position: absolute;
    top: 30px;
    right: 0px;
    border: 1px solid black;
}
.search button{
    width: 50px;
    height: 48px;
    box-sizing: border-box;
    position: absolute;
    top: 31px;
    right: 1px;
    border: 1px solid transparent;
    border-left: 1px solid black;
}
.search input::placeholder{
    padding-left:  10px;
}


</style>