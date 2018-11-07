<style lang="sass">
    @import url('https://use.fontawesome.com/releases/v5.3.1/css/all.css')
    @import "./assets/style/main.sass"
    @import "./assets/style/media.sass"
</style>
<template>
  <div id="app">
    <goods></goods>
    <goods-button></goods-button>
    <ingridient-result></ingridient-result>
  </div>
</template>

<script>
import fetchData from './api/goods.json'
import Goods from "./components/Goods.vue"
import GoodsButton from "./components/GoodsButton.vue"
import IngridientResult from "./components/IngridientResult.vue"


export default {
  name: 'app',
  components: {
  	Goods,
    GoodsButton,
    IngridientResult,
  },
};
</script>


