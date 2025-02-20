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
                <p>Hello dear, my name is jeffery sobaeh, i live in lagos nigeria,<br> i love to too make the web beautiful, alive
                    and yet simple for the avarage user, <br>i love to work as team and bring to live your own website that matches 
                    your brand and style.<br> I also love too worship jesus, read(a liitle), and i am also into forex trading, so yeah,hire me
                </p>
                <div class="wrapper">
                    <div class="skill">
                        <h3>web design</h3>
                        <p>the most modern and high-quality design made at professional level, using modern frame works
                            like vujs, for fanstactic and appealing designs. form all things web2 to web3
                        </p>
                    </div>
                    <div class="experince">
                        <h3>web development</h3>
                        <p>i have a passion for building inovative digital solutons.
                            with exprence in HtmlL,CSS,Javascript,and frame works like
                            vuejs which used i in building this, i craft responsive, scalable,
                            and user-friendly websites and applications.
                        </p>
                    </div>
                    <div class="education">
                        <h3>entraprenur</h3>
                        <p>get proffestional insights from the forex market, from when to buy and sell
                        . get quality web3 service, from all you need to know about the blockchain technology and how it works.
                        </p>
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
    padding-top: 20px;
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
    box-shadow: 0px 10px 20px rgba(0,0,0,0.2);
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
    /* box-shadow: 0px 10px 20px rgba(60,64,67,0.15);
    background: rgb(20, 19, 19); */
    padding-inline: 20px;
    border-bottom: 3px solid teal;
    border-radius: 2px;
    padding-top: 20px;
    border-radius: 5px;
    transition: 0.5s ease;
    box-shadow: inset 0 0 0.5px 1px hsla(0, 0%,  
              100%, 0.075),
              /* shadow ring 👇 */
              0 0 0 1px hsla(0, 0%, 0%, 0.05),
              /* multiple soft shadows 👇 */
              0 0.3px 0.4px hsla(0, 0%, 0%, 0.02),
              0 0.9px 1.5px hsla(0, 0%, 0%, 0.045),
              0 3.5px 6px hsla(0, 0%, 0%, 0.09);

}
h3{
    padding-bottom: 10px;
}
.education:hover{
    border-bottom: 3px solid snow;
}
.experince:hover{
    border-bottom: 3px solid snow;
}
.skill:hover{
    border-bottom: 3px solid snow;
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

@media (max-width:768px){
    .content{
        flex-direction: column;
        gap: 20px;
    }
    .wrapper{
        flex-wrap: wrap;
    }
    
}

</style>