<script setup>
import img1 from '@/assets/img/pic1.jpg'
import img2 from '@/assets/img/pic2.jpg'
import img3 from '@/assets/img/pic3.jpg'
</script>


<template>
<div class="wrapper">
    <div class="content">
        <h1>my work</h1>
    </div>
    <div class="samples">
            <div class="sample">
                <img :src="img1" alt="">
                <div class="overlay">
                    <h1 class="card-title">eagle</h1>
                    <p>simple but yet stunning landing page for a travel agency.
                    </p>
                    <a href="https://audleyjeffery.github.io/netflixclone/"></a>
                </div>
            </div>
            <div class="sample">
                <img :src="img2" alt="">
                <div class="overlay">
                    <h1 class="card-title">vteach</h1>
                    <p>vteach is an educational paltfrom for online learning, i buit multiple pages and made the whole responsiveness<br></p>
                </div>
            </div>
            <div class="sample">
                <img :src="img3" alt="">
                <div class="overlay">
                    <h1 class="card-title">interior paradise</h1>
                    <p>an e commerce website that provide inerior services to all people of every places</p>
                </div>
            </div>
        </div>
</div>
</template>

<style scoped>
.wrapper{
    width: 100%;
    background: black;
    color: snow;
    padding-bottom: 20px;
}
.wrapper .content{
    text-transform: capitalize;
    /* padding: 20px 10px 20px 30px; */
}
.wrapper h1{
    padding-inline: 80px;
    padding-block: 20px;
}

.samples{
    display: flex;
    justify-content: space-around;
    align-items: center;
    position: relative;
    padding-inline: 30px;
}
.sample{
    width: 300px;
    height: 360px;
    overflow: hidden;
    border-radius: 20px;
    position: relative;
    /* box-shadow: 3px 3px 3px rgba(0,0,0,0.7); */
    border: 2px solid teal;
    box-shadow: inset 0 0 0.5px 1px hsla(0, 0%,  
              100%, 0.075),
              /* shadow ring 👇 */
              0 0 0 1px hsla(0, 0%, 0%, 0.05),
              /* multiple soft shadows 👇 */
              0 0.3px 0.4px hsla(0, 0%, 0%, 0.02),
              0 0.9px 1.5px hsla(0, 0%, 0%, 0.045),
              0 3.5px 6px hsla(0, 0%, 0%, 0.09);
}

.sample img{
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 10px;
}
.overlay{
    height: 100%;
    width: 100%;
    background: rgba(9, 20, 46, 0.6);
    bottom: -100%;
    display: grid;
    place-content: center;
    position: absolute;
    text-align: center;
    color: snow;
    border-radius: 10px;
    text-transform: capitalize;
    transition: 0.5s;
}
.card-title{
    padding-bottom: 10px;
}
.sample:hover .overlay{
    bottom: 0;
}
p{
    padding: 10px 10px 0 10px;
}

@media(max-width:768px){
    .samples{
        flex-direction: column;
        gap: 30px;
    }
    h1{
        text-align: center;
    }
}

</style>