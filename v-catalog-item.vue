<template>
    <div class="v-catalog-item">
        <img src="" alt="img">
        <p class="v-catalog-item_name">{{ product_data.name }}</p>
        <p class="v-catalog-item_price">{{ product_data.price }}</p>
        <button class="v-catalog-item_add_to_card_btn btn">купить</button>   
 </div>
</template>

<script>
export default {
    name: "v-catalog-item",
    props: {
        product_data:{
            type: Object,
            default(){
                return{}
            }
        }
    },
    data(){
        return{}
    },
    componed: {

    }
}   
</script>

<style lang="scss">
$padding: 10px;
$margin: 20px;

.v-catalog-item {
    flex-basis: 25%;
    box-shadow: 0 0 8px 0 #e0e0e0;
    padding: 10px;
    margin-bottom: 5px;
    &__image {
      width: 100px;
    }
  }
</style>