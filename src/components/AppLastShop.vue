<template>
	<div class="card-body d-flex text-center my-5 mx-3 pt-1 lastShopCard position-relative">
		<i class="fa-sharp fa-solid fa-cart-shopping my-position"></i>
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
	width: calc(100% / 4);
}

.lastShopCard> div> img{
	width: 300px;
}

.my-position{
	display: none;
	transition: 0.8s;
}
.card-body:hover .my-position{
	font-size: 3rem;
	position: absolute;
	text-align: center;
	color: rgb(196, 191, 191);
	height: 100%;
	width: 100%;
	background-color: rgba(0, 0, 0, 0.507);
	display: flex;
	align-items: center;
	justify-content: center;
	transition: 0.8s;

}
</style>