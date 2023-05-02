<template>
	<header>
		<div>
			<appHeader />
		</div>
	</header>
	<appMain />
	<appFooter />
</template>


<script>
import appHeader from './components/AppHeader.vue';
import appMain from './components/AppMain.vue';
import appFooter from './components/AppFooter.vue';
export default {
	name: 'app',
	components: {
		appHeader,
		appMain,
		appFooter
	},
}
</script>


<style lang="scss" scoped></style>
