<script setup>
</script>

<template>
    <div class="container">
        <h2>my services</h2>
        <div class="content">
            <div class="card">
                <div class="icon">
                    <img src="" class="logo" alt="">
                </div>
                <h3>web developer</h3>
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Atque ipsa quia asperiores laudantium provident ad tempore quam blanditiis neque iure.</p>
                <div class="button">
                        <button class="btn">
                            learn more
                        </button>
                     </div>
            </div>
            <div class="card">
                <div class="icon">
                    <img :src="img1" class="logo" alt="">
                </div>
                <h3>web developer</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem, adipisci? Dignissimos, ea delectus? Distinctio doloribus deserunt quos magni ipsum dolor!</p>
                <div class="button">
                        <button class="btn">
                            learn more
                        </button>
                     </div>
            </div>
            <div class="card">
                <div class="icon">
                    <img :src="img1"  alt="">
                </div>
                <h3>web developer</h3>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Accusantium ratione
                     ea quidem mollitia aliquam reprehenderit repudiandae veritatis alias eveniet et?</p>
                     <div class="button">
                        <button class="btn">
                            learn more
                        </button>
                     </div>
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
    padding: 20px  10px 20px 10px;
    font-size: 30px;
}
.content{
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.card{
    width: 300px;
    height: 300px;
    color: snow;
    border: 1px solid teal;
    padding-inline: 20px;
    border-radius: 10px;
    animation: appaer 10s ease-in-out infinite 1s;
    background: rgba(24, 23, 23, 0.507);
    box-shadow: 0px 1px 2px 0px rgba(60,64,67,0.3),
                0px 2px 6px 2px rgba(60,64,67,0.15);
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
}
.icon img{
    width: 60px;
    height: 60px;
    object-fit: cover;
}
.icon{
    padding-block: 10px;
}
</style>