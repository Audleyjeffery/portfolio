<script setup>

</script>

<template>
    <div class="container">
        <div class="logo">
            <h1>jeffery <span>.</span></h1>
        </div>
        <div class="links">
            <ul>
                <a href="" ><li>Home</li></a>
                <a href="#container" ><li>about</li></a>
                <a href="" ><li>service</li></a>
                <a href="" ><li>portfolio</li></a>
                <a href="" ><li>contact</li></a>
            </ul>
        </div>
    </div>
</template>
<style scoped>
.container{
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding-inline: 20px;
    background: black;
    padding-inline: 50px;
    padding-block: 10px;
}
 .logo h1{
    color: #0f76ac;
    text-transform: capitalize;
    font: 200;
}
.logo span{
    font-size: 60px;
    color: snow;
}
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
}
.links ul a:hover{
    color: teal;
}
</style>