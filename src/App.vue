<template>
	<header>
		<div>
			<ciao />
		</div>
	</header>
</template>


<script>
import linkHeader from './assets/store';
import ciao from './components/AppHeader.vue'
export default {
	name: 'app',
	components: {
		ciao,
	}
}
</script>


<style scoped></style>
