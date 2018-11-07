<template>
	<div class="container">
		<h1>Pizza select!</h1>
	</div>
</template>


<script>
import fetchData from '../api/goods.json'

export default {
	name: 'Goods',
	data() {
		return {
			items: fetchData,
		}
	}
}

</script>