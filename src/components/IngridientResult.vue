<template>
	<div>
		<p v-if="!ingridients.length">No results for ingridient!</p>
		<div v-if="ingridients.length" class="result_ing">
			<ul class="ing_list">
				<li
					v-for="ing in ingridients"
					:key="ing.id"
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
	name: 'IngridientResult',
	data() {
		return {
			ingridients: fetchData,
		}
	}
}

</script>