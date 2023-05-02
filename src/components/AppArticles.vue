<template>
	<div>
		<div class="w-100">
			<img class="w-100" :src="image" :alt="date">
		</div>
		<div class="p-3">
			<h4 class="m-0">
				{{ caption }}
			</h4>
		</div>
		<div class="px-3">
			<span class="text-secondary">
				{{ date }}
			</span>
		</div>
	</div>
</template>

<script>
	export default {
		name:'appArticles',
		props: ['image', 'caption', 'date']
	}
</script>

<style lang="scss" scoped>

</style>