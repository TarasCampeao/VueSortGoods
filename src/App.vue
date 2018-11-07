<style lang="sass">
    @import url('https://use.fontawesome.com/releases/v5.3.1/css/all.css')
    @import "./assets/style/main.sass"
    @import "./assets/style/media.sass"
</style>
<template>
  <div id="app">
    <goods></goods>
  </div>
</template>

<script>
import fetchData from './api/goods.json'
import Goods from "./components/Goods.vue"


export default {
  name: 'app',
  components: {
  	Goods,
  },
};
</script>


