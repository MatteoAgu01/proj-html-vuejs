<template>
	<div class="card-body d-flex my-bg-dark-green p-3 py-5 m-2 mb-5">
		<div>
			<h3 class="text-capitalize text-white py-3">{{ name }}</h3>
			<p class="text-capitalize my-text-green fw-bold">{{ caption }}</p>
		</div>
		<div>
			<img class="food-img" :src="image" :alt="name">
		</div>
		<div class="py-3">
			<button class="my-bg-green border-0 p-2 button-my-bg-green">shop  {{ type }} food</button>
		</div>
	</div>
</template>

<script>
export default {
name: 'foodCard',
props:['name','image','caption', 'type' ]
}
</script>

<style lang="scss" scoped>

// my variables 
$myLifthGrey:	#f9f5f2;
$myGray:		#f2f3f2;
$myLifthGreen:	#3d6f42;
$myGreen:		#1e3120;
//end my variables

.my-text-green{
color: #3d6f42;
}

.my-text-dark-green{
color: #1e3120;
}

.my-bg-green{
	background-color: #3d6f42;
	color: #f2f3f2;
}
.my-bg-dark-green{
	background-color: #1e3120;
	background-image: url(../../public/image-pet/bg-transparent-3.png);
	background-repeat: repeat;
}

.food-img{
	width: 250px;
}
</style>