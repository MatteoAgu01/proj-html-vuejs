<template>
	<div class="my-5">
		<div class="d-flex w-100 mt-5">
			<div class="popular p-5 w-50 text-center d-flex flex-column justify-content-center align-items-center gap-5">
				<p class="text-ppercase text-white fw-bold">
					Lorem ipsum dolor sit amet.
				</p>
				<h2 class="text-white">Popular accesories</h2>
				<button class="p-3 px-5 border-0 rounded-pill bg-body-ligth">view all toys accesoris</button>
			</div>
			<div class="food w-50  p-5 text-center d-flex flex-column justify-content-center align-items-center gap-5">
				<p class="text-ppercase text-white fw-bold">
					Lorem ipsum dolor sit amet.
				</p>
				<h2 class="text-white">new food arrival</h2>
				<button class="p-3 px-2 w-25 border-0 rounded-pill bg-body-ligth">view all food producs</button>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: 'appAccesories'
}
</script>

<style lang="scss" scoped>
.popular {
	background-image: url(../../public/image-pet/banner-last-image/banner-8-2x.jpg);
	filter: grayscale(50%);
	background-position: center;
	background-repeat: no-repeat;
	background-size: cover;
}

.food {
	background-image: url(../../public/image-pet/banner-last-image/banner-9-2x.jpg);
	filter: grayscale(30%);
	background-position: center;
	background-repeat: no-repeat;
	background-size: cover;
}
</style>