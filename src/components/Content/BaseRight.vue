<script setup>
import { onMounted, ref } from "@vue/runtime-core"

const props = defineProps(["images","hasSmallPic"])
let imgIndex = ref(8)
onMounted(() =>{
    imgIndex.value = props.hasSmallPic ? 7 : 8
    console.log(props.hasSmallPic );
    console.log(imgIndex.value);
})

</script>

<template>
<div class="imgbox right">

        <ul>
            <li class ="left" v-for="(img,index) in images.BigPic" :key="index">
            <a href="" v-if="index < imgIndex">
                <div class="pic">
                    <img :src="img.url" alt="">
                </div>
                <h3>{{img.title}}</h3>
                <p>{{img.descripe}}</p>
                <p class="num"><span>{{img.price}}</span>元<span>起</span></p>
                </a>

                <ul class="smallPic" v-if="index >=imgIndex">
                    <li>
                        <a href="">
                       <div class="right"><img :src="images.smallPic.url" alt=""></div>
                        <h4>{{images.smallPic.descripe}}</h4>
                        <p>{{images.smallPic.price}}</p>
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <div class="more">浏览更多</div>
                        </a>
                    </li>
                </ul>
            </li>


        </ul>
    </div>

  
</template>



<style scoped>
.imgbox{
    width: 1026px;
    height: 614px;
    background-color: #F5F5F5;
    
}
ul{
    margin-left: 2px;
}

ul li {
    margin-left: 21px;
    margin-bottom: 14px;
}

ul li a{
    display: block;
    width: 235px;
    height: 300px;
    background-color: #fff;
    text-align: center;
}
.pic img{
    width: 160px;
    height: 160px;
    margin-top: 20px;
}
ul li h3{
    color: #333333;
    margin-top: 20px;
    font-weight: 300;
    font-size: 14px;
    
}
ul li p{
    font-size: 12px;
    color: #b0b0b0;
    margin: 10px 0px;
    overflow: hidden;
	text-overflow:ellipsis;
	white-space: nowrap;
    padding: 0px 10px;
}
ul li .num{
    text-align: center;
    color: #ff6700;
}
.smallPic li{
    background-color: #fff;
    margin-left: 0px;
    margin-bottom: 14px;
    
}
.smallPic img{
    width: 80px;
    height: 80px;
}
.smallPic li a{
    width: 200px;
    height: 143px;
    color: #333333;
    text-align: left;
    padding-left: 20px;
}
.smallPic .more{
    font-size: 18px;
    padding-top: 60px;
    color: #333333;
}
</style>