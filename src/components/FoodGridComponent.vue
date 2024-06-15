
<template>
    <section>
        <slot></slot>
    </section>
</template>

<script>
    export default {
        name: 'FoodGridComponent'
    }
</script>

<style scoped>

    section {
        max-width: 1200px;
        margin: 0 auto;
        padding: 0 24px;
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 16px;
    }
    
</style>