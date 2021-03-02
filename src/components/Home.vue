<template>
	<div>
		<Header />
		<Hero />
		<div class="py-24">
			<div class="container">
				<div class="flex items-center justify-center text-center">
					<div class="w-6/12">
						<h2 class="mb-6 leading-tight text-4xl text-gray-700">Practical projects to get you ahead.</h2>
						<p class="text-lg font-medium text-gray-500">Rather than just teach theory, we focus on real code to inspire your next project. Learning shouldn't be boring, so let's have some fun.</p>
					</div>
				</div>
			</div>
		</div>
		<Testimony />
		<LatestContent />
	</div>
</template>

<script>
	import Header from './Header.vue'
	import Hero from './Hero.vue'
	import Testimony from './Testimony.vue'
	import LatestContent from './LatestContent.vue'

	export default {
		components: {
			Header,
			Hero,
			Testimony,
			LatestContent
		}
	}
</script>

<style></style>
