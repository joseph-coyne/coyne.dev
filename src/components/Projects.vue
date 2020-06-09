<template>
  <div class="block">
    <h2 class="font text-3xl mb-12">Projects</h2>
  <div class="flex justify-between items-center bg-gray-200 rounded py-1 md:py-0 my-2 px-2" v-for="project in projects" :key="project.id">
    <div class="font px-2 w-40 md:w-24">{{ project.name }}</div>
    <div class="hidden md:inline text-gray-700 text-center px-4 py-2 m-2">{{ project.bio }}</div>
    <a :href="project.link" target="_blank" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-1 px-4 rounded">
      Link
    </a>
  </div>
  </div>
</template>

<script>
  export default {
    name: "Projects",
    data() {
      return {
        projects: [
          {
            name: "Spark Fitness",
            bio: "An app for personal trainers and clients to find and schedule workouts.",
            link: "https://github.com/josephpcoyne/fitness-application"
          },
          {
            name: "coyne.dev",
            bio: "This website! An experiement with using TailwindCSS for the first time.",
            link: "https://github.com/josephpcoyne/coyne.dev"
          },
          {
            name: "Vue RPG",
            bio: "A classic RPG game built with Vue.js during a speedrun development.",
            link: "https://github.com/josephpcoyne/vue-rpg"
          }
        ]
      }
    },
  }
</script>

<style scoped>

</style>