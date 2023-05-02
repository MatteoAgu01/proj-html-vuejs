<template>
	<div class="card-body d-flex text-center mt-5 pt-3 lastShopCard">
		<div>
			<img :src="image" :alt="name">
		</div>
		<div>
			<h4 class="text-capitalize text-center">{{ name }}</h4>
			<div class="text-center">
				<span class="d-none">{{ originalPrice }}</span>
				<p class="m-0 my-text-green">{{ currency }} {{ price }}</p>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name:'appLastShop',
	props:['image', 'name', 'originalPrice', 'price', 'currency']

}
</script>

<style lang="scss" scoped>
.lastShopCard{
	width: calc(100% / 3);
}

.lastShopCard> div> img{
	width: 300px;
}
</style>