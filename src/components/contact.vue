<script setup>
import facebook from '@/assets/img/icons8-facebook-50.png'
import insta from '@/assets/img/icons8-instagram-50.png'
import whatlogo from '@/assets/img/icons8-whatsapp-50.png'
import phone from '@/assets/img/icons8-phone-50.png'
import gmail from '@/assets/img/icons8-gmail-50.png'

import { ref } from 'vue';
const whalink = ref('https://wa.link/mrhg54')
const facebooklink = ref('https://facebook.com/Audleyjeffery')
const instalink = ref('https://instagram.com/Audleyjeffery')

</script>

<template>
    <div class="wrapper">
        <h2>contact me</h2>
        <div class="content">
            <div class="contact">
                <div class="gmail">
                    <img :src="gmail" alt="">
                    <h3>jefferysobaeh@gmail.com</h3>
                </div>
                <div class="phone">
                    <img :src="phone" alt="">
                    <h3>09052602298</h3>
                </div>
                <div class="socials">
                    <a :href="facebooklink"><img :src="facebook" alt=""></a>
                   <a :href="instalink"><img :src="insta" alt=""></a>
                    <a :href="whalink"><img :src="whatlogo" alt=""></a>
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
    padding-left: 80px;
    padding-top: 20px;
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
    color: snow;
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
    padding: 10px;
    color: snow;
    resize: none;

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

@media(max-width:768px){
    .content{
        flex-direction: column;
        text-align: center;
        gap: 30px;
    }
    .socials{
        justify-content: center;
        text-align: center;
    }
    .gmail, .phone{
        justify-content: center;
        align-items: normal;
    }

    .inptt1, .inptt2{
        width: 350px;
    }
    .imput{
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
    }
    h2{
        text-align: center;
        padding-inline: 0;
    }
}

</style>