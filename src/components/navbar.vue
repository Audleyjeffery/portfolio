<script setup>
import { ref } from 'vue';


const clicked = ref(false)
const close = ref (false)

const toggleopen = () =>{
    if(clicked.value === false){
        clicked.value = true
        close.value = true
    }
    else{
        clicked.value = false
        close.value = false
    }
}

</script>

<template>
    <div class="container">
        <div class="logo">
            <h1>jeffery <span>.</span></h1>
        </div>
        <div :class="{click: clicked}" class="links" >
            <ul>
                <a href="" ><li>Home</li></a>
                <a href="#container" ><li>about</li></a>
                <a href="" ><li>service</li></a>
                <a href="" ><li>portfolio</li></a>
                <a href="" ><li>contact</li></a>
            </ul>
        </div>
        <div id="links" >
            <ul>
                <a href="" ><li>Home</li></a>
                <a href="#container" ><li>about</li></a>
                <a href="" ><li>service</li></a>
                <a href="" ><li>portfolio</li></a>
                <a href="" ><li>contact</li></a>
            </ul>
        </div>
        <div @click="toggleopen" class="harm" :class="{closed: close}">
            <div class="btn-line"></div>
            <div class="btn-line"></div>
             <div class="btn-line"></div>
            </div>
    </div>
</template>
<style scoped>
.container{
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: black;
    padding-inline: 50px;
    padding-block: 10px;
}
 .logo h1{
    color: teal;
    text-transform: capitalize;
    font: 200;
}
.logo span{
    font-size: 60px;
    color: snow;
}
/* harmburger menu */
.links ul{
    display: flex;
    align-items: center;
    gap: 20px;
    padding: 20px;
    color: snow;
}
.links ul a{
    text-decoration: none;
    font-size: 20px;
    text-transform: capitalize;
    outline: none;
    color: snow;
    list-style: none;
    text-align: center;
    transition: 0.3s ease-in-out;
}
.links ul a:hover{
    color: teal;
}
.links{
    display: none;
}
/* harmburger menu ends here */
#links ul{
    display: flex;
    align-items: center;
    gap: 20px;
    padding: 20px;
    color: snow;
}
#links ul a{
    text-decoration: none;
    font-size: 20px;
    text-transform: capitalize;
    outline: none;
    color: snow;
    list-style: none;
    text-align: center;
    transition: 0.3s ease-in-out;
}
#links ul a:hover{
    color: teal;
}

.harm{
    display: none;
    transition: 0.5s;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}
.closed{
    transform: rotate(180deg);
}

.btn-line{
    width: 25px;
    height: 4px;
    margin: 0 0 5px 0;
    transition: 0.5s;
    background-color: snow;
}
.closed .btn-line:nth-child(1){
    transform:  rotate(45deg) translate(5px , 5px);
}
.closed .btn-line:nth-child(2){
    opacity: 0;
}
.closed .btn-line:nth-child(3){
    transform:  rotate(-45deg) translate(7px , -8px);
}

@media(max-width:768px){
    .harm{
        display: block;
    }
    #links{
        display: none;
    }
    
    .links{
        position: fixed;
        top: 0;
        left: 0;
        width: 0;
        z-index: 3;
        overflow: hidden;
        display: block;
        transition: 0.4s ease;
    }
    .click{
        width: 16rem;
        overflow: none;
    }
    .links ul{
        flex-direction: column;
        padding-block: 0;
        background: rgb(26, 45, 45);
        padding-block: 30px;
        height: 60vh;
    }
}
</style>