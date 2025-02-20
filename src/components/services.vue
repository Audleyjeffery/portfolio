<script setup>
import blockchain from '@/assets/img/icons8-bitcoin-cryptocurrency-50.png'
import webdesign from '@/assets/img/icons8-web-design-50.png'
import website from '@/assets/img/icons8-web-development-50.png'
</script>

<template>
    <div class="container">
        <h2>my services</h2>
        <div class="content">
            <div class="card" id="card">
                <div class="icon">
                    <img :src="blockchain" class="logo" alt="">
                </div>
                <h3>forex/blochain technology</h3>
                <p>explore the web3, get familar with blockchain technology.
                    how it works, the hypes and trend of things, get the bset services, 
                    community management, content writting, trading and airdrops.
                    learn when to buy and sell in the forex market.
                </p>
                <!-- <div class="button">
                        <button class="btn">
                            learn more
                        </button>
                     </div> -->
            </div>
            <div class="card">
                <div class="icon">
                    <img :src="webdesign" class="logo" alt="">
                </div>
                <h3>web design</h3>
                <p> get scalable and modern designs,all things web2 to web3, 
                    from beautiful product design to the most attaracting landing pages.</p>
                <!-- <div class="button">
                        <button class="btn">
                            learn more
                        </button>
                     </div> -->
            </div>
            <div class="card" id="card">
                <div class="icon">
                    <img :src="website"  alt="">
                </div>
                <h3>web development</h3>
                <p>get a full and functional websites of your choice, built to your liking with the 
                    most morden technology, from all things web2 t0 web3 using the best frontend tools down to the back end. easy for user to
                    interact with and navigate.
                </p>
                     <!-- <div class="button">
                        <button class="btn">
                            learn more
                        </button>
                     </div> -->
            </div>
        </div>
    </div>
</template>
<style scoped>
.container{
    width: 100%;
    background: black;
    color: snow;
    text-transform: capitalize;
    padding: 50px 30px 50px 30px;
}
h2{
    padding: 20px  10px 20px 50px;
    font-size: 30px;
}
.content{
    display: flex;
    align-items: center;
    justify-content: space-around;
}
.card{
    width: 300px;
    height: 330px;
    color: snow;
    padding-top: 20px;
    /* border: 1px solid teal; */
    padding-inline: 20px;
    border-radius: 10px;
    transition: 0.5s ease;
    /* animation: appaer 10s ease-in-out infinite 1s; */
    /* background: rgba(24, 23, 23, 0.507); */
              /* inner glow 👇 */
    box-shadow: inset 0 0 0.5px 1px hsla(0, 0%,  
              100%, 0.075),
              /* shadow ring 👇 */
              0 0 0 1px hsla(0, 0%, 0%, 0.05),
              /* multiple soft shadows 👇 */
              0 0.3px 0.4px hsla(0, 0%, 0%, 0.02),
              0 0.9px 1.5px hsla(0, 0%, 0%, 0.045),
              0 3.5px 6px hsla(0, 0%, 0%, 0.09);
}
.card:hover{
    border: 2px solid teal;
}
@keyframes appaer{
    0%{
    border: 2px solid teal;
    }
    40%{
        border-top: 2px solid snow;

    }
    60%{
        border-right: 2px solid yellow;

    }
    60%{
        border-bottom: 2px solid palevioletred;

    }
    80%{
        border-left: 2px solid yellow;
    }
    
    100%{
        border-top: 2px solid teal;
    }
}
.card h2{
    padding-block: 20px;
    font-size: 20px;
}
.card p{
    padding-block: 20px;
}
.btn{
    font-size: 18px;
    text-transform: capitalize;
    padding: 10px 20px 10px 20px;
    outline: none;
    border-radius: 5px;
    margin-bottom: 30px;
}
.icon img{
    width: 60px;
    height: 60px;
    object-fit: cover;
}
.icon{
    padding-block: 10px;
}
@media(max-width:768px){
    .content{
        flex-direction: column;
        gap: 30px;
    }
    h2{
        text-align: center;
        padding-inline: 0;
    }
}
</style>