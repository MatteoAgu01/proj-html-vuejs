<template>
	<div class="banner-bg mt-5 d-flex flex-column align-items-center justify-content-center">
		<section class="my-arrivals-sec text-white d-flex flex-column align-items-center justify-content-center gap-4 p-5">
			<h6 class="text-uppercase">find the best animals supplies</h6>
			<h2 class="fs-1">New arrivals weekly</h2>
			<button class="border-0 rounded-pill p-2 px-4">
				Learn more about us
			</button>
		</section>
	</div>
</template>

<script>
export default {
	name: 'appArrivals',
}
</script>

<style lang="scss" scoped>
.banner-bg{
	background-image: url(../../public/image-pet/new-arrivals-bg/banner-3-2x-scaled.jpg);
	background-position: center;
	background-size: cover;
	height: 60vh;
	min-height: 200px;
	filter: grayscale(20%);
}
.my-arrivals-sec{
	background-color: rgba(0, 0, 0, 0.418);
	border-radius: 20px;
}

</style>