<template>
	<nav class="mb-10"
	:class="[ currentRoute ? 'nav-white' : 'nav-blue']">
		<div class="mx-auto max-w-screen-lg">
			<div class="flex items-center sm:p-3 justify-between overflow-visible px-4">
				<router-link to="/" class="sm:p-2 font-medium text-md sm:text-xl leading-6">
					<!-- <img
						class="hidden sm:inline mb-2 h-12 w-12"
						src="../assets/images/logo.png"
						alt="Logo"
					/> -->
					Joseph Coyne
				</router-link>
				<!-- Mobile menu toggle -->
				<div
					@click="isOpen = !isOpen"
					class="sm:hidden text-3xl inline-block items-center p-2"
				>
					<span v-if="!isOpen"> = </span>
					<span v-if="isOpen"> × </span>
				</div>

				<div class="hidden font-medium sm:inline justify-between items-center">
					<router-link
						to="/about"
						class="font-open font-semibold m-2 px-5 py-3 rounded active:shadow-md">
              About
            </router-link>
					<!-- <router-link to="/blog" class="text-center px-4 py-2 m-2">Blog</router-link>    -->
					<router-link 
          to="/contact" 
					class="font-open font-semibold m-2 px-5 py-3 rounded active:shadow-md">
            Contact
          </router-link>
				</div>
			</div>
			<div
				:class="isOpen ? 'block' : 'hidden'"
				class="sm:hidden font-medium w-full absolute bg-blue-800 flex z-10 border-t-2"
			>
				<router-link to="/about" class="text-center px-4 py-2 m-2">
					<span @click="close()">About</span>
				</router-link>
				<router-link
					@click="close()"
					to="/contact"
					class="text-center px-4 py-2 m-2"
				>
					<span @click="close()">Contact</span>
				</router-link>
			</div>
		</div>
	</nav>
</template>

<script>
export default {
	name: 'NavBar',
	data() {
		return {
			isOpen: false
		};
	},
	methods: {
		close() {
			this.isOpen = false;
		}
	},
	computed: {
    currentRoute() {
      return this.$route.name === 'Login' || this.$route.name === 'Admin'
    }
  },
};
</script>

<style scoped>

</style>
