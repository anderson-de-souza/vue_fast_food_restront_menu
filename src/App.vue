
<template>

    <HeaderComponent title="Food Mixing" />

    <FoodGridComponent>
        <FoodCardComponent 
          v-for="(food, index) of foodList" 
          :foodImageSource="food['foodImageSource']"
          :foodName="food['foodName']"
          :foodPrice="food['foodPrice']" 
          :key="index" />
    </FoodGridComponent>

    <FooterComponent />

</template>

<script>
    
    import HeaderComponent from './components/HeaderComponent.vue'
    import FoodGridComponent from './components/FoodGridComponent.vue'
    import FoodCardComponent from './components/FoodCardComponent.vue'
    import FooterComponent from './components/FooterComponent.vue'

    import Foods from './foods.json'

    export default {
      name: 'App',
      components: {
        HeaderComponent,
        FoodGridComponent,
        FoodCardComponent,
        FooterComponent
      },
      data() {
        return {
          foodList: Foods
        }
      }
    }
</script>

<style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, Helvetica, sans-serif;
    }
</style>
