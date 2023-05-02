<template>
	<footer class="text-white my-bg-dark-green py-5 mt-3">
		<div class="d-flex w-75 m-auto justify-content-around border-bottom border-color-ligth py-5">
			<div>
				<img src="../../public/image-pet/logo/mobile-light-pet-logo-2x-200x52.png" alt="white-logo">
				<p class="p-2">1234 avada Avenue Avadaville <br>
					info@your-company.com <br>
					call us (1) 234 5678
				</p>
			</div>
			<div class="text-white">
				<ul>
					<li class="text-capitalize text-white">
						<h5>shop by brand</h5>
					</li>
					<li class="text-capitalize text-white">Bed</li>
					<li class="text-capitalize text-white">food</li>
					<li class="text-capitalize text-white">toys</li>
					<li class="text-capitalize text-white">trasport</li>
				</ul>
			</div>
			<div class="text-white">
				<ul>
					<li class="text-capitalize text-white">
						<h5>useful links</h5>
					</li>
					<li class="text-capitalize text-white">my account</li>
					<li class="text-capitalize text-white">orders</li>
					<li class="text-capitalize text-white">checkout</li>
					<li class="text-capitalize text-white">cart</li>
				</ul>
			</div>

			<div class=" bg-image text-white p-3">
				<p class="fw-bold">subcribe to our news letter</p>
				<input class="bg-body-ligth border-0 rounded-pill px-3 py-1 my-3" type="email" name="" id=""
					placeholder="insert your email...*"> <br>
				<button class="border-0 rounded-pill px-3 py-1 my-3 my-bg-green">subcribe</button>
			</div>
		</div>
		<div class="py-3">
			<div class="d-flex justify-content-center">
				<ul class="d-flex border-bottom border-color-ligth py-3">
					<li><span class="text-white text-capitalize p-3 mx-3">home</span></li>
					<li><span class="text-white text-capitalize p-3 mx-3">about</span></li>
					<li><span class="text-white text-capitalize p-3 mx-3">blog</span></li>
					<li><span class="text-white text-capitalize p-3 mx-3">conctat</span></li>
					<li><span class="text-white text-capitalize p-3 mx-3">shop</span></li>
				</ul>
			</div>
			<div class="d-flex justify-content-center">
				<i class="fa-brands fa-facebook mx-1 p-2"></i>
				<i class="fa-brands fa-twitter mx-1 p-2"></i>
				<i class="fa-brands fa-instagram mx-1 p-2"></i>
				<i class="fa-brands fa-youtube mx-1 p-2"></i>
			</div>
		</div>
	</footer>
</template>

<script>
export default {
	name: 'appFooter'
}
</script>

<style lang="scss" scoped>
.bg-image {
	background-image: url(../../public/image-pet/bg-transparent-3.png);
	background-color: rgb(20, 54, 20);
}
</style>