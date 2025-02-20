<script setup>
import im2 from '@/assets/img/FB.jpg'
import facebook from '@/assets/img/icons8-facebook-50.png'
import insta from '@/assets/img/icons8-instagram-50.png'
import whatlogo from '@/assets/img/icons8-whatsapp-50.png'

import { ref } from 'vue';
const whalink = ref('https://wa.link/mrhg54')
const facebooklink = ref('https://facebook.com/Audley.jeffery.7')
const instalink = ref('https://instagram.com/Audleyjeffery')
</script>

<template>
    <div class="container">
        <div class="content">
            <div class="info">
                <h2> <span>jeffery  </span>sobaeh</h2>
                <h4>web developer | python programmer | entraprenur</h4>
                <p>Hi, my name is jeffery sobaeh, i am from lagos nigeria,<br> and i dabble in all things web development</p>
                <div class="socials">
                    <a :href="facebooklink"><img :src="facebook" alt=""></a>
                   <a :href="instalink"><img :src="insta" alt=""></a>
                    <a :href="whalink"><img :src="whatlogo" alt=""></a>
                </div>
                <div class="btn">
                    <a :href="whalink"><button>hire me</button></a>
                </div>
            </div>
            <div class="profile">
                <div class="wrapper">
                    <img :src="im2" alt="">
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>
.container{
    width: 100%;
    background: black;
}
.content{
    display: flex;
    align-items: center;
    justify-content: space-around;
    padding-block: 60px;
    color: snow;
    text-transform: capitalize;
    padding-inline: 60px;
}
.info{
    /* width: 500px;
    height: 400px; */
    display: grid;
    place-content: center;

}
h2{
    width: 100%;
    font-size: 60px;
}
.info h4{
    width: 100%;
    font-size: 20px;
    padding-block: 10px;
}
p{
    text-transform: none;
    padding-right: 20px;
}
.wrapper{
    width: 300px;
    height: 300px;
    overflow: hidden;
    border-radius: 50%;
    border: 8px solid snow;
    box-shadow: 2px 2px 6px rgba(67,67,67,0.3);
}
.wrapper img{
    width: 300px;
    height: 300px;
    object-fit: cover;
    border-radius: 50%;
}
.wrapper:hover{
    border: 8px solid teal;
}
span{
    color: teal;
}
.socials{
    display: flex;
    align-items: center;
    gap: 20px;
    padding-block: 20px;
}
.socials img{
    width: 30px;
    height: 30px;
}
.btn button{
    padding: 10px 20px 10px 20px;
    font-size: 20px;
    letter-spacing: 2px;
    text-transform: capitalize;
    color: teal;
    border: 1px solid snow;
    border-radius: 1px;
    background: transparent;
    transition: 0.8s ease;
}
.btn button:hover{
    background: snow;
    color: black;
}
@media (max-width:760px){
    .content{
        flex-direction: column;
        align-items: center;
        justify-content: center;
        text-align: center;
    }
    .info{
        order: 1;
    }
    .wrapper{
        margin-bottom: 20px;
    }
    .socials{
        justify-content: center;
        align-items: center;
    }
}

</style>