<template>
	<main>
		<div class="text-center w-50 m-auto py-2 my-4">
			<h2 class="text-capitalize">
				brows by category
			</h2>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate, laborum? Alias voluptate ex
				laudantium aperiam dignissimos non corporis quis perspiciatis.
			</p>
		</div>
		<div class="d-flex justify-content-around p-4 mb-3">
			<firstCardSec :image="firstCard.image" :alt="firstCard.alt" :shop="firstCard.shop.length"
				v-for="(firstCard, index) in card" :key="index" class="d-flex flex-column align-items-center gap-4" />
		</div>
		<div class="d-flex justify-content-around gap-4 pt-4">
			<foodCard :image="food.image" :name="food.name" :caption="food.caption" :type="food.type"
				v-for="(food, index) in foodCardCom" :key="index"
				class="d-flex flex-column align-items-center text-center gap-4" />
		</div>
		<div>
			<appArrivals />
		</div>
		<div class="py-5 ">
			<div>
				<p class="fw-bold fs-5 my-green">All-time best sellers</p>
				<h2 class="fs-1">Items everyone loves</h2>
			</div>
			<div class="d-flex justify-content-around gap-4">
				<appGadgetOne :image="gadgetOne.image" :name="gadgetOne.name" :originalPrice="gadgetOne.origi"
					:price="gadgetOne.price" :currency="gadgetOne.currency" v-for="(gadgetOne, index) in firstShop"
					:key="index" class="d-flex flex-column align-items-center gap-4 " />
			</div>
		</div>
		<div>
			<div id="bg-image" class="pt-5 bg-image my-4 position-relative">
				<div class="text-center">
					<h2 class="text-white p-3">User testimonials</h2>
				</div>
				<div class="d-flex justify-content-between bg-green p-2">
					<appTestimonials :image="testimonials.image" :caption="testimonials.caption"
						:name="testimonials.name" :theme="testimonials.theme"
						v-for="(testimonials, index) in userTestimonials" :key="index"
						class="text-center m-2 pb-5 d-flex justify-content-center my-card" />
				</div>

			</div>
				<appMail />
		</div>
	</main>
</template>

<script>
import { firstCard } from '../assets/store';
import { food } from '../assets/store';
import { gadgetOne } from '../assets/store';
import { testimonials } from '../assets/store';
import firstCardSec from './AppCard.vue';
import foodCard from './AppCardFood.vue';
import appArrivals from './AppNewArrivals.vue';
import appGadgetOne from './AppGadgetOne.vue';
import appTestimonials from './AppTestimonials.vue';
import appMail from './AppMail.vue';
export default {
	name: 'appMain',
	data() {
		return {
			card: firstCard,
			foodCardCom: food,
			firstShop: gadgetOne,
			userTestimonials: testimonials

		}
	},
	components: {
		firstCardSec,
		foodCard,
		appArrivals,
		appGadgetOne,
		appTestimonials,
		appMail,
	},
}


</script>

<style lang="scss" scoped>
.my-green {
	color: #3d6f42;
}

#bg-image {
	background: rgb(30, 49, 32);
	background-image: url(../../public/image-pet/bg-transparent-3.png);
}

.bg-green {
	background: rgb(30, 49, 32);
	background: linear-gradient(180deg, rgba(30, 49, 32, 0.719) 0%, rgba(30, 49, 32, 0.801) 13%, rgba(30, 49, 32, 0.8575805322128851) 29%, rgba(30, 49, 32, 0.925) 55%, rgba(30, 49, 32, 1) 73%);
}

.my-card {
	width: calc(100% / 3);
	padding: 10px;
}

.my-card img {
	width: 50px;
}
</style>