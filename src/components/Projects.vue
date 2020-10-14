<template>
	<section class="my-2 sm:py-16 ">
		<h2 class="font-semibold text-3xl mb-12">Projects</h2>
		<div class="flex flex-col">
			<div
				class="bg-gray-200 justify between rounded my-2 py-2 px-4 "
				v-for="(project, i) in projects"
				:key="i"
			>
        <div class="flex flex-wrap flex-row-reverse sm:flex-row justify-between items-center py-2 bg-gray-200 rounded sm:py-0 my-1 sm:my-2 pb-4 overflow-y-hidden transition-all duration-200"
        ref="projects"
        :class="[isOpen === i ? maxHeight : 'max-h-10']">
          <h1 class="font-semibold whitespace-no-wrap order-2 sm:order-1">{{ project.name }}</h1>
          <p class=" sm:inline order-2 py-4 sm:py-0 text-gray-700 sm:whitespace-no-wrap">
            {{ project.bio }} 
          </p>

          <!-- <p class="sm:hidden py-2 order-2 text-gray-700 sm:text-center">
            {{ project.bio }}
          </p> -->
    
          <a
            :href="project.link"
            target="_blank"
            class=" btn btn-blue mr-1 sm:mr-1 order-3 sm:order-2"
          >
            <span class="px-1 font-open font-semibold">
              Link
            </span>
            <i class="fab fa-github px-1"></i>
          </a>
          <button class="sm:hidden order-1"
            @click="toggleAccordion(i)">
            <i
              class="p-1 outline-none text-blue-800 fas fa-chevron-down"
            ></i>
          </button>
          
        </div>
      </div>
		</div>
	
	</section>
</template>

<script>
export default {
	name: 'Projects',
	data() {
		return {
			isOpen: null,
			maxHeight: 'max-h-10',
			projects: [
				{
					name: 'Spark Fitness',
					bio:
						'Application for personal trainers and clients to find and schedule workouts.',
					link: 'https://github.com/joseph-coyne/fitness-application'
				},
				{
					name: 'coyne.dev',
					bio:
						'This website! An experiemental playground for any new tech I want to try.',
					link: 'https://github.com/joseph-coyne/coyne.dev'
				},
				{
					name: 'Vue RPG',
					bio:
						'A classic RPG game built with Vue.js during a speedrun development.',
					link: 'https://github.com/joseph-coyne/vue-rpg'
				}
			]
		};
	},
	methods: {
		toggleAccordion(i) {
      if(this.isOpen != i){
        this.isOpen = i;
        var rems = Object.keys(this.$tw.theme.spacing).map(Number);
        var h = this.$refs.projects[i].scrollHeight / 16;
        h = h * 4;
        var nh = rems.sort((a, b) => Math.abs(h - a) - Math.abs(h - b))[0];
        
        this.isOpen === i
          ? (this.maxHeight = 'max-h-' + nh)
          : (this.maxHeight = 'max-h-10');
      } else {
        this.isOpen = null;
      }
		}
	},
	computed: {}
};
</script>

<style scoped>

</style>
