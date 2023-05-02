<template>
	<div>
		<div class="m-0">
			<div class="d-flex flex-column justify-content-end">
				<div class="m-1 p-2">
					<img class="rounded-circle my-test-img" :src="image" :alt="name">
				</div>
				<div class="m-1 p-2">
					<p class="text-white m">{{ caption }}</p>
				</div>
				<div class="m-1 p-2">
					<span class="text-secondary">{{ name }},{{ theme }}</span>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: 'appTestimonials',
	props: ['image', 'caption', 'name', 'theme']
}
</script>

<style lang="scss" scoped>
.my-test-img{
	width:100px;
}
</style>