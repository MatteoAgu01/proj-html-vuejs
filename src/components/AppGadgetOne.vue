<template>
	<div class="card-body d-flex text-center mt-5 pt-3">
		<div>
			<img :src="image" :alt="name">
		</div>
		<div>
			<h4 class="text-capitalize text-center">{{ name }}</h4>
			<div class="text-center">
				<span class="d-none">{{ originalPrice }}</span>
				<p class="m-0 my-green">{{ currency }} {{ price }}</p>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name:'appGadgetOne',
	props:['image', 'name', 'originalPrice', 'price', 'currency']
}
</script>

<style lang="scss" scoped></style>