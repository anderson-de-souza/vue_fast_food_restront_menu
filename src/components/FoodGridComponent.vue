
<template>
    <section>
        <div>
            <slot></slot>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'FoodGridComponent'
    }
</script>

<style scoped>

    section {
        width: 100vw;
        min-height: 980px;
        background-color: black;
    }


    div {
        width: 80%;
        min-height: 100%;
        margin: 0 auto;
    }

    slot {
        min-width: 100%;
        min-height: 100%;
        display: grid;
    }

</style>