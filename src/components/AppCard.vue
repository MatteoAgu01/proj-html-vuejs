<template>
	
		<div class="card-body d-flex">
			<div>
				<img :src="image" :alt="alt">
			</div>
			<div>
				<h4 class="text-capitalize">{{ alt }}({{ shop }})</h4>
			</div>
		</div>
	
</template>

<script>
export default {
	name: 'firstCardSec',
	props:['image','alt','shop'],
}
</script>

<style lang="scss" scoped></style>