<template>
	<main>
		<div class="text-center w-50 m-auto py-2 my-4">
			<h2 class="text-capitalize">
				brows by category
			</h2>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate, laborum? Alias voluptate ex laudantium aperiam dignissimos non corporis quis perspiciatis.
			</p>
		</div>
		<div class="d-flex justify-content-around p-4 mb-3">
			<firstCardSec :image="firstCard.image" :alt="firstCard.alt" :shop="firstCard.shop.length" v-for="(firstCard, index) in card" :key="index"
				class="d-flex flex-column align-items-center gap-4"/>
		</div>
		<div class="d-flex justify-content-around gap-4 pt-4">
			<foodCard :image="food.image" :name="food.name" :caption="food.caption" :type="food.type" v-for="(food, index) in foodCardCom" :key="index"
				class="d-flex flex-column align-items-center text-center gap-4"/>
		</div>
	</main>
</template>

<script>
import { firstCard } from '../assets/store'
import {food} from '../assets/store'
import firstCardSec from './AppCard.vue'
import foodCard from './AppCardFood.vue'
export default {
	name: 'appMain',
	data() {
		return {
			card: firstCard,
			foodCardCom:food
		}
	},
	components: {
		firstCardSec,
		foodCard,
	}
}

</script>

<style lang="scss" scoped></style>