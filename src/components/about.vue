<script setup>
import img1  from'@/assets/img/FB.jpg'
</script>

<template>
    <div class="#container">
        <div class="content">
            <div class="img left">
                <div class="imgcon">
                    <img :src="img1" alt="">
                </div>
            </div>
            <div class="text">
                <h2>about me</h2>
                <p>Hello dear, my name is jeffery sobaeh, i am from lagos nigeria,<br> i love to too make the web beautiful, alive
                    and yet simple for the avarage user, <br>i love to work as team and bring to live your own website that matches 
                    your brand and style.<br> I also love too worship jesus, read(a liitle), and i am also into forex trading, so yeah,hire me
                </p>
                <div class="info">
                    <h3>skill</h3>
                    <h3>exprience</h3>
                    <h3>education</h3>
                </div>
                <div class="wrapper">
                    <div class="skill">
                        <h3>web developer</h3>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat odit tempore 
                            illo consequatur vero velit, dolorem quasi dignissimos cupiditate quibusdam.</p>
                    </div>
                    <div class="experince">
                        <h3>web developer</h3>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat odit tempore 
                            illo consequatur vero velit, dolorem quasi dignissimos cupiditate quibusdam.</p>
                    </div>
                    <div class="education">
                        <h3>web developer</h3>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat odit tempore 
                            illo consequatur vero velit, dolorem quasi dignissimos cupiditate quibusdam.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>
#container{
    width: 100%;
}
.wrapper{
    width: 100%;
    display: flex;
    align-items: center;
    /* justify-content: space-between; */
    gap: 50px;
}
.content{
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 100px;
    padding-inline: 80px;
    text-transform: capitalize;
    background: black;
    color: snow;
    padding-block: 30px;
}
.text h2{
    font-size: 30px;
    padding-bottom: 10px;
    color: #0f76ac;
}

h3{
    cursor: pointer;
}

ul li{
    display: flex;
    flex-direction: column;
    gap: 10px;
    list-style: none;
}
.img{
    width: 300px;
    height: 300px;
    background: rgb(20, 19, 19);
    display: grid;
    place-content: center;
    overflow: hidden;
    border-radius: 10px;
    border: 8px solid teal;
}
.imgcon{
    width: 300px;
    height: 100%;
    padding-inline: 10px;
    box-shadow: 2px 6px 2px 6px rgba(60,64,67,0.15);
}
.imgcon img{
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 10px;
}

.education, .experince, .skill{
    width: 300px;
    height: 200px;
    box-shadow: 2px 6px 2px 6px rgba(60,64,67,0.15);
    background: rgb(20, 19, 19);
    padding-inline: 20px;
    border-bottom: 3px solid teal;
    border-radius: 2px;
    padding-top: 20px;
}
h3{
    padding-bottom: 10px;
}
.info{
    display: flex;
    align-items: center;
    /* justify-content: space-between; */
    padding-block: 20px;
    gap: 100px;
}
ul li{
    padding-block: 3px;
}
ul span{
    color: tomato;
}
@keyframes appaer{
    0%{
    border: 8px solid teal;
    }
    40%{
        border: 8px solid snow;

    }
    60%{
        border: 8px solid yellow;

    }
    
    100%{
        border: 8px solid teal;
    }
}
.left{
    animation: appaer 0.8s ease infinite 5s;
}

</style>
<script>
export default {
    setup() {
        const skill = document.querySelector('.ski')
        const education =document.querySelector('.education');
        const exprience = document.querySelector('.experience')

skill.addEventListener('click',() =>{
    education.style.display= 'none'
    exprience.style.display='none'
})
    },
}
</script>