<template>
    <div id="main-banner">
        <h1>Make Your Burger</h1>
    </div>
</template>

<script>
export default {
    name: 'Banner'
}
</script>

<style scoped>

    #main-banner {
        position: relative;
        overflow: hidden; 
        height: 500px;
        display: flex;
        align-items: center;
        justify-content: flex-start;
    }

    #main-banner::before {
        content: ''; 
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-image: url('/img/burger.jpg');
        background-size: cover;
        z-index: -1; 
        transition: transform 0.4s ease-out;
    }

    #main-banner h1{
        color: #FFF;
        text-align: center;
        font-size: 60px;
        background-color: #222;
    }

</style>