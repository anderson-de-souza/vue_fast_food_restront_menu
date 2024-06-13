
<template>
    <div class="card">
        <img :src="foodImageSource">
        <div>
            <h2>{{ foodName }}</h2>
            <h3>{{ foodPrice }}</h3>
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
        width: 300px;
        min-width: 300px;
        min-height: 380px;
        background-color: antiquewhite;
        display: flex;
        align-items: end;
        justify-content: end;
        position: relative;
    }

    img {
        position: absolute;
        width: 100%;
        height: 100%;
        max-width: 100%;
        max-height: 100%;
    }

</style>