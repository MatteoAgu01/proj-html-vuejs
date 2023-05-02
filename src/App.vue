<template>
	<header>
		<div>
			<appHeader />
		</div>
	</header>
	<appMain />
</template>


<script>
import appHeader from './components/AppHeader.vue'
import appMain from './components/AppMain.vue';
export default {
	name: 'app',
	components: {
		appHeader,
		appMain,
	},
}
</script>


<style lang="scss" scoped></style>
