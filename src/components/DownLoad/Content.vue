<script setup>

</script>

<template>
<div class="content">
    <div class="container">
        <div class="download">
                    <div class="pc-img">
                        <img src="https://www-growth.scdn.co/static/download/laptop.svg" alt="">
                    </div>
                    <h1>DownLoad Spotify</h1>
                    <p>Play millions of songs and podcasts on your device.</p>
                        <button class="dLink">
                            DownLoad
                        </button>
        </div>

        <div class="Store">
            <h3>Bring your music to mobile and tablet, too.</h3>
            <p>Listening on your phone or tablet is free, easy and fun.</p>
            <div class="imgBox">
              
                   <a href=""><img src="https://www-growth.scdn.co/static/badges/svgs/apple/badge-en.svg" alt=""></a>
                    <a href=""><img src="https://www-growth.scdn.co/static/badges/svgs/google/badge-en.svg" alt=""></a>
                    <a href=""><img src="https://www-growth.scdn.co/static/badges/microsoft-windows/en.png" alt=""></a>
              
            </div>
        </div>
        <div class="descripe">
            <div>
                <img src="https://www-growth.scdn.co/static/download/all-devices.svg" alt="">
            </div>
            <h3>One account, listen everywhere.</h3>
            <div class="platform">
                <ul>
                    <li class="left"><span>MOBLE</span></li>
                    <li class="left"><span>COMPUTER</span></li>
                    <li class="left"><span>TABLE</span></li>
                    <li class="left"><span>CAR</span></li>
                    <li class="left"><span>PLAYSTATION</span></li>
                    <li class="left"><span>XBOX</span></li>
                    <li class="left"><span>TV</span></li>
                    <li class="left"><span>SPEAKER</span></li>
                    <li class="left"><span>WEB PLAYER</span></li>
                </ul>
            </div>
        </div>
    </div>
</div>

  
</template>

<style scoped>

.download{
    height: 450px;
    background-color: #19E68C;
    text-align: center;
}
.pc-img img{
    width: 136px;
    height: 80px;
    margin-top: 80px;
    margin-bottom: 40px;
}
.download h1{
    font-size: 40px;
    margin-bottom: 20px;
}
.download button{
    width: 138px;
    height: 48px;
    border-radius: 100px;
    border: 1px solid transparent;
    font-weight: 700;
    background-color: #FFFFFF;
    margin-top: 30px;
}

.Store{
    height: 200px;
    text-align: center;
}
.Store h3{
    font-weight: 700;
    font-size: 32px;
    margin-top: 50px;
}
.Store p{
    font-size: 16px;
    font-weight: 400;
    margin-top: 20px;
}
.imgBox img {
    width: 120px;
    height: 40px;
    margin-top: 20px;
}
.imgBox a{
    margin-left: 20px;
    padding-left: 12px;
}
.descripe{
    height: 480px;
    text-align: center;
    background-color: #222326;
    color: white;
}
.descripe img {
    width: 480px;
    height: 174px;
    margin-top: 60px;
}
.descripe h3 {
    font-size: 32px;
    margin-top: 20px;
}
.descripe ul {
    list-style-type: disc;
    width: 800px;
    margin-top: 30px;

}
.descripe ul li {
   text-align: -webkit-match-parent;
   margin-left: 30px;
   list-style: inside;
}

.platform{
    display: inline-block;
    text-align: center;
}

</style>