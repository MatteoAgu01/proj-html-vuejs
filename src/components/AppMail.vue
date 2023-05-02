<template>
	<div class="bg-news w-75 my-0 mx-auto p-5">
		<div>
			<h2 class="disply-1 p-3">join our newsletter</h2>
			<p class="w-50 p-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur illum magnam est eveniet inventore illo
				neque delectus, assumenda reprehenderit sapiente?
			</p>
		</div>
		<div>
			<input class="rounded-pill border-0 mail-grey p-3 px-5 mx-2" type="email" name="" id="" placeholder="insert your mail...*">
			<button class="text-white p-3 px-5 mx-2 border-0 rounded-pill my-bg-green">subcribe</button>
		</div>
	</div>
</template>

<script>
export default {
	name: 'appMail'
}
</script>

<style lang="scss" scoped>
.bg-news{
	background-image: url(../../public/image-pet/sand-message-bg/banner-7-2x-scaled.jpg);
	background-size: cover;
	position: relative;
	bottom:80px;
}

.mail-grey{
	background-color: #f2f3f2;
}

</style>