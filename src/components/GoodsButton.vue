<template>
	<div class="container goods_zone">
		<ul class="add_list">
			<li v-for="(item, value) in items" :key="item.id">
				<button class="btn_goods">{{ value }}</button>
			</li>
		</ul>
	</div>
</template>


<script>
import fetchData from '../api/goods.json'
	
export default {
	name: 'GoodsButton',
	data() {
		return {
			items: fetchData,
		}
	}
}


</script>