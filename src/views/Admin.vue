<template>
  <main class="flex flex-col mt-12 md:max-w-3xl mx-auto">
    <section class="pt-12 mt-2 md:py-16">
			<div class="flex flex-wrap">
				<div class="w-full flex flex-col">
					<ul class="flex mb-0 list-none flex-wrap pb-4 flex-row">
						<li class="-mb-px mr-2 last:mr-0 flex-auto text-center">
							<a class="text-xs font-bold uppercase px-5 py-3 shadow-lg rounded block leading-normal cursor-pointer" v-on:click="toggleTabs(1)" 	
							:class="{'text-blue-800 bg-white': openTab !== 1, 'text-white bg-indigo-700': openTab === 1}">
								Home
							</a>
						</li>
						<li class="-mb-px mr-2 last:mr-0 flex-auto text-center">
							<a class="text-xs font-bold uppercase px-5 py-3 shadow-lg rounded block leading-normal cursor-pointer" v-on:click="toggleTabs(2)" 
							:class="{'text-blue-800 bg-white': openTab !== 2, 'text-white bg-indigo-700': openTab === 2}">
								Projects
							</a>
						</li>
						<li class="-mb-px mr-2 last:mr-0 flex-auto text-center">
							<a class="text-xs font-bold uppercase px-5 py-3 shadow-lg rounded block leading-normal cursor-pointer" v-on:click="toggleTabs(3)" 
							:class="{'text-blue-800 bg-white': openTab !== 3, 'text-white bg-indigo-700': openTab === 3}">
								About
							</a>
						</li>
						<li class="-mb-px mr-2 last:mr-0 flex-auto text-center">
							<a class="text-xs font-bold uppercase px-5 py-3 shadow-lg rounded block leading-normal cursor-pointer" v-on:click="toggleTabs(4)" 
							:class="{'text-blue-800 bg-white': openTab !== 4, 'text-white bg-indigo-700': openTab === 4}">
								Contact
							</a>
						</li>
					</ul>
					<div class="tab-content tab-space">
						<div :class="{'hidden': openTab !== 1, 'block': openTab === 1}">
							<div class="flex flex-row bg-white w-full rounded-t border-b justify-between">
								<h1 class="text-lg text-gray-700 m-2 p-2">Edit Home page</h1>
								<button class="bg-indigo-500 place-self-center text-white active:bg-indigo-600 font-bold uppercase text-xs px-4 py-2 rounded shadow hover:shadow-md mr-4  ease-linear transition-all duration-150" type="button">
									Save
								</button>
							</div>
							<div class="relative min-w-0 break-words bg-gray-200 w-full mb-6 rounded-b">
								<div class="px-8 py-8 flex-auto">
									<div class="flex justify-center">
										<div class="flex flex-col w-2/6 mr-10 mt-2">
											<img src="@/assets/images/headshot-cropped.png" alt="Upload a picture" 
											class="shadow rounded max-w-s max-h-s object-cover align-middle border-none mb-4" />
											<button class="w-32 bg-indigo-500 place-self-center text-white active:bg-indigo-600 font-bold uppercase text-xs px-4 py-2 rounded shadow hover:shadow-md mr-1 mb-1 ease-linear transition-all duration-150" type="button">
												Upload Photo
											</button>
										</div>
										<div class="w-3/6 ml-10">
											<h1 class="text-lg text-gray-700 pb-2">Header</h1>
											<textarea  placeholder="Header" class="resize-none px-3 py-3 placeholder-gray-400 text-gray-700 relative bg-white rounded text-sm shadow focus:outline-none w-full h-24"></textarea>
											<h1 class="text-lg text-gray-700 py-2 mt-2">Body</h1>
											<textarea  placeholder="Body" class="resize-none px-3 py-3 placeholder-gray-400 text-gray-700 relative bg-white rounded text-sm shadow focus:outline-none w-full h-24"></textarea>
										</div>
									</div>
								</div>
							</div>
						</div>
						<div :class="{'hidden': openTab !== 2, 'block': openTab === 2}">
							<div class="flex flex-row bg-white w-full rounded-t border-b justify-between">
								<h1 class="text-lg text-gray-700 m-2 p-2">Edit Projects</h1>
								<button class="bg-indigo-500 place-self-center text-white active:bg-indigo-600 font-bold uppercase text-xs px-4 py-2 rounded shadow hover:shadow-md mr-4  ease-linear transition-all duration-150" type="button">
									Save
								</button>
							</div>
							<div class="relative min-w-0 break-words bg-gray-200 w-full mb-6 rounded-b">
								<div class="px-8 py-8 flex-auto">
									<div class="flex justify-center">
										<div class="flex flex-col w-2/6 mr-10 mt-2">
											<img src="" alt="Upload a picture" 
											class="shadow rounded object-cover max-w-s max-h-s bg-white align-middle border-none mb-4" />
											<button class="w-32 bg-indigo-500 place-self-center text-white active:bg-indigo-600 font-bold uppercase text-xs px-4 py-2 rounded shadow hover:shadow-md mr-1 mb-1 ease-linear transition-all duration-150" type="button">
												Upload Photo
											</button>
										</div>
										<div class="w-3/6 ml-10">
											<h1 class="text-lg text-gray-700 pb-2">Title</h1>
											<input type="text"  placeholder="Title" class="resize-none px-3 py-3 placeholder-gray-400 text-gray-700 relative bg-white rounded text-sm shadow focus:outline-none w-full">
											<h1 class="text-lg text-gray-700 py-2 mt-2">Description</h1>
											<textarea  placeholder="Description" class="resize-none px-3 py-3 placeholder-gray-400 text-gray-700 relative bg-white rounded text-sm shadow focus:outline-none w-full h-24"></textarea>
										</div>
									</div>
								</div>
							</div>
						</div>
						<div :class="{'hidden': openTab !== 3, 'block': openTab === 3}">
							<div class="flex flex-row bg-white w-full rounded-t border-b justify-between">
								<h1 class="text-lg text-gray-700 m-2 p-2">Edit About page</h1>
								<button class="bg-indigo-500 place-self-center text-white active:bg-indigo-600 font-bold uppercase text-xs px-4 py-2 rounded shadow hover:shadow-md mr-4 ease-linear transition-all duration-150" type="button">
									Save
								</button>
							</div>
							<div class="relative min-w-0 break-words bg-gray-200 w-full mb-6 rounded-b">
								<div class="px-8 py-8 flex-auto">
									<div class="flex justify-center">
										<div class="flex flex-col w-2/6 mr-10 mt-2">
											<img src="@/assets/images/luna.jpg" alt="Upload a picture" 
											class="shadow rounded max-w-s max-h-s object-cover align-middle border-none mb-4" />
											<button class="w-32 bg-indigo-500 place-self-center text-white active:bg-indigo-600 font-bold uppercase text-xs px-4 py-2 rounded shadow hover:shadow-md mr-1 mb-1 ease-linear transition-all duration-150" type="button">
												Upload Photo
											</button>
										</div>
										<div class="w-3/6 ml-10">
											<h1 class="text-lg text-gray-700 pb-2">Header</h1>
											<textarea  placeholder="Header" class="resize-none px-3 py-3 placeholder-gray-400 text-gray-700 relative bg-white rounded text-sm shadow focus:outline-none w-full h-24"></textarea>
											<h1 class="text-lg text-gray-700 py-2 mt-2">Body</h1>
											<textarea  placeholder="Body" class="resize-none px-3 py-3 placeholder-gray-400 text-gray-700 relative bg-white rounded text-sm shadow focus:outline-none w-full h-24"></textarea>
										</div>
									</div>
								</div>
							</div>
						</div>
						<div :class="{'hidden': openTab !== 4, 'block': openTab === 4}">
							<div class="flex flex-row bg-white w-full rounded-t border-b justify-between">
								<h1 class="text-lg text-gray-700 m-2 p-2">Edit Contact page</h1>
								<button class="bg-indigo-500 place-self-center text-white active:bg-indigo-600 font-bold uppercase text-xs px-4 py-2 rounded shadow hover:shadow-md mr-4  ease-linear transition-all duration-150" type="button">
									Save
								</button>
							</div>
							<div class="relative min-w-0 break-words bg-gray-200 w-full mb-6 rounded-b">
								<div class="px-8 py-8 flex-auto">
									<div class="flex justify-center">
										<div class="w-3/6 ml-10">
											<h1 class="text-lg text-gray-700 pb-2">Body</h1>
											<textarea  placeholder="Header" class="resize-none px-3 py-3 placeholder-gray-400 text-gray-700 relative bg-white rounded text-sm shadow focus:outline-none w-full h-24"></textarea>
										</div>
									</div>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
    </section>
  </main>
</template>

<script>
  export default {
    name: "Admin",
    data() {
    return {
      openTab: 1
    }
  },
  methods: {
    toggleTabs: function(tabNumber){
      this.openTab = tabNumber
    }
  }
  }
</script>

<style scoped>

</style>