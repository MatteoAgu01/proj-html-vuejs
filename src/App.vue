<template>
	<header>
		<div>
			<ciao />
		</div>
	</header>
	<appMain/>
</template>


<script>
import ciao from './components/AppHeader.vue'
import appMain from './components/AppMain.vue';
export default {
	name: 'app',
	components: {
		ciao,
		appMain,
	}
}
</script>


<style lang="scss" scoped>

</style>
