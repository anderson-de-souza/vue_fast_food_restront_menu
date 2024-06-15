
<template>
    <div class="card">
        <img :src="foodImageSource">
        <div class="info">
            <h2 class="text">{{ foodName }}</h2>
            <h3 class="text">{{ foodPrice }}</h3>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'FoodCardComponent',
        props: {
            foodName: String,
            foodImageSource: String,
            foodPrice: String
        }
    }
</script>

<style scoped>

    .card {
        width: 100%;
        height: 420px;
        position: relative;
        border-radius: 16px;
        overflow: hidden;
    }

    img {
        width: 100%;
        height: 100%;
    }

    .info {
        padding: 10px;
        background-color: rgba(0, 0, 0, 0.4);
        position: absolute;
        left: 0;
        bottom: 0;
    }

    .text {
        background-color: rgba(0, 0, 0, 0);
        color: aliceblue;
    }

    .info:hover {
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
    }

    
</style>