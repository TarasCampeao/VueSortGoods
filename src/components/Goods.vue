<template>
	<div class="container">
		<h1>Pizza select!</h1>
	    <goods-button></goods-button>
	    <div class="info_group">
	    	<ingridient-result></ingridient-result>
	    	<goods-selected></goods-selected>	    	
	    </div>
	</div>
</template>


<script>
import fetchData from '../api/goods.json'
import GoodsButton from "../components/GoodsButton.vue"
import IngridientResult from "../components/IngridientResult.vue"
import GoodsSelected from "../components/GoodsSelected.vue"

export default {
	name: 'Goods',
	components: {
		GoodsButton,
		IngridientResult,
		GoodsSelected,
	},
	data() {
		return {
			items: fetchData,
		}
	}
}

</script>