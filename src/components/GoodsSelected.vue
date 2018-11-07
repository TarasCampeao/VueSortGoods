<template>
	<div class="select_result">
		<p v-if="!selected.length">No selected goods!</p>
		<div v-if="selected.length" class="result_ing">
			<ul class="ing_list">
				<li
					v-for="select in selected"
					:key="select.id"
				>
					{{ value }}
				</li>
			</ul>
		</div>
	</div>
</template>


<script>
import fetchData from '../api/goods.json'	


export default {
	name: 'GoodsSelected',
	data() {
		return {
			selected: fetchData,
		}
	}
}

</script>