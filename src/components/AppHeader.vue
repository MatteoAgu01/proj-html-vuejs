<template>
	<div>
		<nav>
			<div class="d-flex align-item-end justify-content-around py-3">
				<div class="d-flex align-item-center">
					<img src="../../public/images/avada-pet-supplies/dark-pet-logo.png" alt="logo">
				</div>
				<div class=" d-flex align-item-baseline border rounded-pill p-2">
					<i class="fa-solid fa-search align-self-center mx-2"></i>
					<input class="border-0 my-searchbar" type="text" placeholder="Search...">
				</div>
				<div class="d-flex align-item-center">
					<p class="align-self-center m-0"><b class="text-capitalize"> questions?</b>Call us : 1.800.123.4567
					</p>
				</div>
				<div class="d-flex align-self-center">
					<i class="fa-regular fa-bag-shopping m-2 align-self-center"></i>
					<i class="fa-regular fa-user m-2 align-self-center"></i>
				</div>
			</div>
			<div class="d-flex justify-content-center">
				<div v-for="(linkHeader, index) in linkNav.linkHeader" @key="index">
					<ul class="">
						<li class="d-flex align-item-center justify-content-center">
							<p class="text-capitalize m-0">
								{{ linkHeader.title }}
							</p>
							<i class="fa-solid fa-chevron-down d-flex align-self-center m-0"></i>
						</li>
					</ul>
				</div>
			</div>
		</nav>
		<div class="myGreen">
			<section class="myTitleSec d-flex flex-column justify-content-end gp-1">
				<div class="d-flex lign-items-center justify-content-evenly py-3">
					<ul class="d-flex">
						<li class="text-white d-flex gap-2 align-items-center">
							<i class="fa-regular fa-map"></i>
							<p class="fw-bold m-0">International </p>
							<span class="text-capitalize text-secondary">shipping service</span> 
						</li>
					</ul>
					<ul class="d-flex">
						<li class="text-white d-flex gap-2 align-items-center">
							<i class="fa-regular fa-clock"></i>
							<span class="text-capitalize text-secondary">see our</span> 
							<p class="fw-bold m-0">store hours </p>
							<span class="text-capitalize text-secondary">and services</span> 
						</li>
					</ul>
					<ul class="d-flex">
						<li class="text-white d-flex gap-2 align-items-center">
							<i class="fa-regular fa-check"></i>
							<span class="text-capitalize text-secondary">we price Lorem ipsum dolor sit.</span> 
							<p class="fw-bold m-0">best deals</p>
						</li>
					</ul>
				</div>
				<div class="myBgTitle p-0 position-relative">
					<img  class="myBgBanner" src="../../public/image-pet/header-image/banner-5-2x-scaled.jpg" alt="bg-banner">
					<div class="myTitleText">
						<p class="fw-bold text-white">Lorem ipsum dolor sit amet.</p>
						<h2 class="text-white">Lorem ipsum dolor sit <br> amet consectetur adipisicing.</h2>
						<div class="my-4">
							<button class="bg-body-white border-0 rounded-pill">
								<h5 class="py-2 px-3 m-0 fs-6">Learn more about us</h5>
							</button>
						</div>
					</div>
				</div>
				<div class="d-flex align-items-end justify-content-end px-3 mt-2">
					<img src="../../public/image-pet/header-image/food-transparent-5-200x112.png" alt="food-heder" class="px-2">
					<p class="text-white m-0 px-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam, dicta.</p>
					<a class="text-bg-tertiary px-2" href="">Visit the shop</a>
				</div>
			</section>
		</div>
	</div>
</template>

<script>
import linkHeader from '../assets/store'

export default {
	name: 'ciao',
	data() {
		return {
			linkNav: linkHeader,
		}
	}

}
</script>


<style lang="scss">
// my variables 
$myLifthGrey: #f9f5f2;
$myGray: #f2f3f2;
$myLifthGreen: #3d6f42;
$myGreen: #1e3120;

//end my variables
.my-searchbar {
	width: 300px;
	background-color: #f9f5f2;
}

ul {
	list-style-type: none;
	color: rgb(150, 147, 147);
}

ul:hover p {
	text-decoration: underline;
	color: black;
}

nav {
	position: fixed;
	top: 0;
	left: 0;
	z-index: 1000;
	width: 100%;
	min-height: 117px;
	background-color: #f2f3f2;
}

.myGreen {
	background-color: #1e3120;
	background-image: url(../../public/image-pet/bg-transparent-3.png);
	background-repeat: repeat;
	margin-top: 120px;
}

.myTitleSec {
	height: 80vh;
	min-height: 300px;
}

.myBgTitle {
	height: 85vh;
	min-height:285px ;
	z-index: 999;
}

.myBgBanner{
	width: 100%;
	margin-bottom: 5px;
	filter: grayscale(40%);
}

.myTitleText{
	position: absolute;
	top: 20%;
	left: 10%;
}
</style>