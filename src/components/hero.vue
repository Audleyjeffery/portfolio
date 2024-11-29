<script setup>
import im2 from '@/assets/img/FB.jpg'
import facebook from '@/assets/img/facebook.png'
import insta from '@/assets/img/insta.png'
import whatlogo from '@/assets/img/whatlogo.png'
</script>

<template>
    <div class="container">
        <div class="content">
            <div class="info left">
                <h4>web developer|python programmer|entranpuer</h4>
                <h2> <span>jeffery  </span>sobaeh</h2>
                <p>hi, my name is jefery sobaeh, i am from lagos nigeria,<br> and i dabble in all things web development</p>
                <div class="socials">
                    <img :src="facebook" alt="">
                    <img :src="insta" alt="">
                    <img :src="whatlogo" alt="">
                </div>
                <div class="btn">
                    <button>hire me</button>
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
.info h3{
    width: 100%;
    font-size: 25px;
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
    color: #0f76ac;
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
    background: #0f76ac;
    color: snow;
    border: none;
    border-radius: 1px;

}
@media (max-width:760px){
    .content{
        flex-direction: column;
    }
    .wrapper{
        order: 0;
    }
}

</style>