<template>
	<div class="my-bg-dark-green img">
		<div class="d-flex flex-column align-items-center gap-3" >
			<i class="fs-2" :class="icon" :style="style" ></i>
			<p class="gray">{{ caption }}</p>
		</div>
	</div>
</template>

<script>
	export default {
		name:'appInfo',
		props: ['icon', 'caption','style']
	}
</script>

<style lang="scss" scoped>
.gray{
	color: rgb(175, 175, 175);
}
</style>