<template>
	<div class="container">
		<h1>Pizza select!</h1>
	    <goods-button></goods-button>
    	<ingridient-result></ingridient-result>
	</div>
</template>


<script>
import fetchData from '../api/goods.json'
import GoodsButton from "../components/GoodsButton.vue"
import IngridientResult from "../components/IngridientResult.vue"

export default {
	name: 'Goods',
	components: {
		GoodsButton,
		IngridientResult,
	},
	data() {
		return {
			items: fetchData,
		}
	}
}

</script>