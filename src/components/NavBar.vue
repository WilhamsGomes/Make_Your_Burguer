<template>
    <nav id="nav">
        <router-link to="/" id="logo-url"> <img :src="logo" :alt="alt"/> </router-link>
        <router-link to="/">Home</router-link> 
        <router-link to="/pedidos">Pedidos</router-link>
    </nav>
</template>

<script>
    export default {
        name:'Navbar',
        props: ["logo", "alt"]
    }
</script>
 
<style scoped>

    #nav{
        background-color: #222;
        
        padding: 15px 50px;
        display: flex;
        justify-content: flex-end;
        align-items: center;
    }

    #nav #logo-url{
        margin: auto;
        margin-left: 0;
    }

    #logo-url img{
        width: 50px;
        height: 50px;
    }

    #nav a{
        color: #FCBA03;
        text-decoration: none;
        margin: 12px;
        transition: .5s;
    }

    #nav a:hover{
        color: #FFF;
    }
 
</style>
