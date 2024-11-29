<script setup>
import img1 from '@/assets/img/pic1.jpeg'
import img2 from '@/assets/img/pic2.jpg'
import img3 from '@/assets/img/pic3.jpeg'
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
                    <h1 class="card-title">living room</h1>
                    <h3 class="title2">
                        observe the best shit man
                    </h3>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quaerat est,
                     magnam nemo eum distinctio dolor consequuntur alias fugiat autem id!</p>
                </div>
            </div>
            <div class="sample">
                <img :src="img2" alt="">
                <div class="overlay">
                    <h1 class="card-title">living room</h1>
                    <h3 class="title2">
                        observe the best shit man
                    </h3>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quaerat est,
                     magnam nemo eum distinctio dolor consequuntur alias fugiat autem id!</p>
                </div>
            </div>
            <div class="sample">
                <img :src="img3" alt="">
                <div class="overlay">
                    <h1 class="card-title">living room</h1>
                    <h3 class="title2">
                        observe the best shit man
                    </h3>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quaerat est,
                     magnam nemo eum distinctio dolor consequuntur alias fugiat autem id!</p>
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
    padding-inline: 30px;
    padding-block: 20px;
}

.samples{
    display: flex;
    justify-content: space-between;
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
    box-shadow: 3px 3px 3px rgba(0,0,0,0.7);
    border: 2px solid teal;
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

</style>