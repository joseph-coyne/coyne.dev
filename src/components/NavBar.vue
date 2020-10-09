<template>
	<nav class="mb-10 bg-blue-800  text-white">
		<div class="mx-auto max-w-screen-lg">
			<div class="flex items-center md:p-3 justify-between overflow-visible px-4">
				<router-link to="/" class="md:p-2 font-medium text-md md:text-xl leading-6">
					<!-- <img
						class="hidden md:inline mb-2 h-12 w-12"
						src="../assets/logo.png"
						alt="Logo"
					/> -->
					Joseph Coyne
				</router-link>
				<!-- Mobile menu toggle -->
				<div
					@click="isOpen = !isOpen"
					class="md:hidden text-3xl inline-block items-center p-2"
				>
					<span v-if="!isOpen"> = </span>
					<span v-if="isOpen"> × </span>
				</div>

				<div class="hidden font-medium md:inline justify-between items-center">
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
				class="md:hidden font-medium w-full absolute bg-blue-800 flex z-10 border-t-2"
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
	}
};
</script>

<style scoped>

</style>
