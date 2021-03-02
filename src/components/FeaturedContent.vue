<template>
	<div class="py-16 relative">
		<div class="container">
			<div class="mb-12 flex justify-between items-end">
				<div>
					<h2 class="text-gray-600 text-3xl font-semibold mb-2">
						Featured content
					</h2> 
					<span class="text-lg text-gray-500 mb-4 font-normal"></span>
				</div> 
			</div>
			<div class="flex flex-wrap -ml-4 -mr-4">
				<div class="w-full flex md:w-full lg:w-1/3 p-4" v-for="item in featured" :key="item.title">
					<div class="relative block">
						<a href="/courses/build-a-file-sharing-saas-app" class="absolute w-full h-full top-0 left-0"></a> 
						<div class="bg-white h-full rounded flex flex-col justify-between items-start p-10">
							<div class="flex flex-wrap pb-24">
								<a href="#" class="" v-for="tag in item.tags" :key="tag">
									<div class="inline-block text-sm font-semibold rounded px-3 py-1 mr-2 mb-2 bg-gray-300 text-gray-600">
										{{ tag }}
									</div>
								</a>
							</div>
							<div>
								<h4 class="text-base font-semibold text-gray-500 capitalize mb-2">
									course
								</h4>
								<h3 class="font-semibold text-lg mb-4">
									{{ item.title }}
								</h3>
								<p class="font-light m-0 text-gray-500">
									{{ item.description }}
								</p>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>
<script>
	export default {
		data() {
			return {
				featured: [
					{
						'tags' : ['Laravel', 'Vue.js'],
						'title': 'Build a File Sharing SaaS App',
						'description' : 'Let’s build a file sharing SaaS app with Laravel and Vue! Featuring direct, signed uploads to S3 with FilePond, secure sharing, tiered pricing plans, usage statistics and more.'
					},
					{
						'tags' : ['Laravel', 'Vue.js'],
						'title': 'Build a File Sharing SaaS App',
						'description' : 'Let’s build a file sharing SaaS app with Laravel and Vue! Featuring direct, signed uploads to S3 with FilePond, secure sharing, tiered pricing plans, usage statistics and more.'
					},
					{
						'tags' : ['Laravel', 'Vue.js'],
						'title': 'Build a File Sharing SaaS App',
						'description' : 'Let’s build a file sharing SaaS app with Laravel and Vue! Featuring direct, signed uploads to S3 with FilePond, secure sharing, tiered pricing plans, usage statistics and more.'
					},
				]
			}
		}
	}
</script>