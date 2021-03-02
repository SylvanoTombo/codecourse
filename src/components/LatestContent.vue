<template>
		<div class="py-24">
			<div class="container">
				<div class="flex items-end justify-between mb-12">
					<div>
						<h2 class="text-gray-600 text-3xl font-semibold mb-2">Latest Content</h2>
						<span class="text-gray-400 text-lg mb-4 font-normal">Fresh from library</span>
					</div>
					<a href="#" class="text-blue-400">Browse everithing &#x2192;</a>
				</div>

				<div class="mb-10">
					<div class="bg-white rounded-lg mb-4"  v-for="lesson in latest" :key="lesson.title">
						<div class="flex flex-wrap">
							<div class="p-8 flex-grow">
								<a href="#">
									<h3 class="text-lg font-semibold mb-4 text-gray-600">{{ lesson.title }}</h3>
								</a>
								<ul class="flex flex-wrap">
									<li class="mr-4 text-gray-500 flex items-center mb-2 font-semibold">
										<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" class="mr-2 w-5 h-5 fill-current text-gray-500"><path d="M12 22a10 10 0 1 1 0-20 10 10 0 0 1 0 20zm0-2a8 8 0 1 0 0-16 8 8 0 0 0 0 16zm1-8.41l2.54 2.53a1 1 0 0 1-1.42 1.42L11.3 12.7A1 1 0 0 1 11 12V8a1 1 0 0 1 2 0v3.59z"></path></svg> <!---->
										{{ lesson.duration }} mins
									</li>
									<li class="mr-4 text-gray-500 flex items-center mb-2 font-semibold">
										<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" class="mr-2 mr-2 w-5 h-5 fill-current text-gray-500"><path d="M17 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V6c0-1.1.9-2 2-2h2V3a1 1 0 1 1 2 0v1h6V3a1 1 0 0 1 2 0v1zm-2 2H9v1a1 1 0 1 1-2 0V6H5v4h14V6h-2v1a1 1 0 0 1-2 0V6zm4 6H5v8h14v-8z"></path></svg>
										<span title="2021-02-26 13:55:00">
											Released 4 days ago
										</span>
									</li>
								</ul>
								<div class="flex flex-wrap mt-4">
									<a class="inline-block text-sm font-semibold rounded px-3 py-1 mr-2 mb-2 bg-gray-200 text-gray-500 hover:bg-gray-500 hover:text-white" href="#" v-for="tag in lesson.tags" :key="tag">{{ tag }}</a>
									<div class="inline-block text-sm font-semibold rounded px-3 py-1 mr-2 mb-2 bg-gray-600 text-gray-100" v-if="lesson.new">New</div>
								</div>
							</div>
						</div>
					</div>
				</div>

				<div>

				</div>
			</div>
			<div class="flex justify-center">
				<a 
					href="#" 
					class="bg-blue-500 px-5 py-4 text-white rounded">
					Browse all courses
				</a>
			</div>
		</div>
</template>

<script>
	export default {
		data () {
			return {
				latest: [
					{
						'title': 'Alpine.js Auto Textarea Height',
						'duration': 6,
						'new': true,
						'tags': ['Alpinejs']
					},
					{
						'title': 'Polling Batched Jobs Progress with Livewire',
						'duration': 31,
						'new': false,
						'tags': ['Laravel', 'Laravel Livewire']
					},
					{
						'title': 'Preventing Duplicate Form Submits in Laravel',
						'duration': 39,
						'new': false,
						'tags': ['Laravel']
					},
					{
						'title': 'Laravel Websockets with Nuxt',
						'duration': 52,
						'new': false,
						'tags': ['Laravel', 'Nuxt']
					},
					{
						'title': 'Switching Exposed Team IDs in Laravel Jetstream',
						'duration': 14,
						'new': false,
						'tags': ['Laravel']
					}
				]
			}
		}
	}
</script>
