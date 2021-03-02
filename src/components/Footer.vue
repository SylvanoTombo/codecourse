<template>
	<div class="bg-gray-800 py-10 lg:py-24">
		<div class="container">
			<div class="flex">
				<div class="lg:w-2/12" v-for="item in items" :key="item.title">
					<h4 class="text-gray-500 uppercase mb-6 text-sm">{{ item.title }}</h4>
					<ul>
						<li v-for="link in item.links" :key="link.title">
							<a 
								:href="link.url" 
								class="block text-gray-300 mb-4 font-semibold">
								{{ link.title }}
							</a>
						</li>
					</ul>
				</div>
			</div>
		</div>
		<div class="container mt-24">
			<div class="text-gray-500 text-sm">
				© 2021 Codecourse Ltd. All Rights Reserved. Born in London, UK.
			</div>
		</div>
	</div>
</template>
<script>
	export default {
		data () {
			return {
				items : [
					{
						'title' : 'Library',
						'links' : [
							{
								'title' : 'Latest & Featured',
								'url' 	: '#',
							},
							{
								'title' : 'Latest & Featured',
								'url' 	: '#',
							},
							{
								'title' : 'Latest & Featured',
								'url' 	: '#',
							},
							{
								'title' : 'Latest & Featured',
								'url' 	: '#',
							},
						]
					},
					{
						'title' : 'Library',
						'links' : [
							{
								'title' : 'Latest & Featured',
								'url' 	: '#',
							},
						]
					},
					{
						'title' : 'Library',
						'links' : [
							{
								'title' : 'Latest & Featured',
								'url' 	: '#',
							},
							{
								'title' : 'Latest & Featured',
								'url' 	: '#',
							},
						]
					},
					{
						'title' : 'Library',
						'links' : [
							{
								'title' : 'Latest & Featured',
								'url' 	: '#',
							},
							{
								'title' : 'Latest & Featured',
								'url' 	: '#',
							},
							{
								'title' : 'Latest & Featured',
								'url' 	: '#',
							},
							{
								'title' : 'Latest & Featured',
								'url' 	: '#',
							},
						]
					},
					{
						'title' : 'Library',
						'links' : [
							{
								'title' : 'Latest & Featured',
								'url' 	: '#',
							},
							{
								'title' : 'Latest & Featured',
								'url' 	: '#',
							},
							{
								'title' : 'Latest & Featured',
								'url' 	: '#',
							},
							{
								'title' : 'Latest & Featured',
								'url' 	: '#',
							},
						]
					},
				]
			}
		}
	}
</script>