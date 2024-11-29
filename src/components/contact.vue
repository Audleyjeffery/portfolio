<script setup>
import facebook from '@/assets/img/facebook.png'
import insta from '@/assets/img/insta.png'
import whatlogo from '@/assets/img/whatlogo.png'
</script>

<template>
    <div class="wrapper">
        <div class="content">
            <div class="contact">
                <h2>contact me</h2>
                <div class="gmail">
                    <img src="" alt="">
                    <h3>jefferysobaeh@gmail.com</h3>
                </div>
                <div class="phone">
                    <img src="" alt="">
                    <h3>09052602298</h3>
                </div>
                <div class="socials">
                    <img :src="facebook" alt="">
                    <img :src="insta" alt="">
                    <img :src="whatlogo" alt="">
                </div>
            </div>
            <div class="imput">
                <div class="inptt1">
                    <input type="text" placeholder="your name">
                </div>
                <div class="inptt1">
                    <input type="text" placeholder="your email">
                </div>
                <div class="inptt2">
                    <textarea name="text" placeholder="write here"></textarea>
                </div>
                <div class="btn">
                    <button>submit</button>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.wrapper{
    width: 100%;
    text-transform: capitalize;
    background: black;
    color: snow;
    padding-bottom: 10px;
}
h2{
    font-size: 30px;
}
.content{
    display: flex;
    /* align-items: center; */
    justify-content: space-around;
    padding-block: 50px;
    color: snow;
}
.inptt1{
    width: 600px;
    height: 40px;
    margin-bottom: 20px;
    background: rgba(24, 23, 23, 0.507);
   
}
input{
    width: 100%;
    height: 100%;
    background: rgba(24, 23, 23, 0.507);
    border: none;
    padding-inline: 10px;
}
.inptt2{
    width: 600px;
    height: 200px;
}
textarea{
    width: 100%;
    height: 100%;
    background: rgba(24, 23, 23, 0.507);
    border: none;
}
.btn{
    padding-block: 20px;
}
.btn button{
    padding: 10px 20px 10px 20px;
    font-size: 18px;
    text-transform: capitalize;
}
.gmail{
    display: flex;
    align-items: center;
    gap: 20px;
    padding-block: 10px;
}
.gmail img{
    width: 20px;
    height: 20px;
}
.phone{
    display: flex;
    align-items: center;
    gap: 20px;
}
.phone img{
    width: 20px;
    height: 20px;
}
.socials{
    display: flex;
    align-items: center;
    gap: 20px;
    padding-block: 10px;
}
.socials img{
    width: 20px;
    height: 20px;
}

</style>