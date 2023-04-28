<template>
	<div>
		<nav class="d-flex align-item-end justify-content-around py-3">
			<div class="d-flex align-item-center">
				<img src="../../public/images/avada-pet-supplies/dark-pet-logo.png" alt="logo">
			</div>
			<div class=" d-flex align-item-baseline border rounded-pill">
				<i class="fa-solid fa-search align-self-center mx-2"></i>
				<input class="border-0 my-searchbar"  type="text" placeholder="Search..." >
			</div>
			<div class="d-flex align-item-center">
				<p class="align-self-center m-0"><b class="text-capitalize"> questions?</b>Call us : 1.800.123.4567</p>
			</div>
			<div class="d-flex align-self-center">
				<i class="fa-regular fa-bag-shopping m-2 align-self-center"></i>
				<i class="fa-regular fa-user m-2 align-self-center"></i>
			</div>
		</nav>
	</div>
</template>

<script>
	export default {
		name:'ciao'
	}
</script>

<style lang="scss" scoped>
	.my-searchbar{
		width: 300px;
	}
</style>