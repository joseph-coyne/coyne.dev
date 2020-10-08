<template>
  <section class="pt-12 mt-2 md:py-16 ">
    <h2 class="font-semibold text-3xl mb-12">Projects</h2>
    <div class="flex flex-col">
      <div
        class="flex justify-between items-center bg-gray-200 rounded my-2 py-2 md:py-0  px-4"
        v-for="project in projects"
        :key="project.id"
      >
        <h1 class="font-semibold whitespace-no-wrap">{{ project.name }}</h1>
        <p class="hidden md:inline text-gray-700 text-center py-2 m-2">{{ project.bio }}</p>
        <a
          :href="project.link"
          target="_blank"
          class="bg-blue-500 hover:bg-blue-400 text-white font-semibold py-1 px-4 rounded"
        >Link</a>
      </div>
    </div>

  </section>
</template>

<script>
export default {
  name: "Projects",
  data() {
    return {
      projects: [
        {
          name: "Spark Fitness",
          bio:
            "Application for personal trainers and clients to find and schedule workouts.",
          link: "https://github.com/josephpcoyne/fitness-application"
        },
        {
          name: "coyne.dev",
          bio:
            "This website! An experiemental playground for any new tech I want to try. Overall I keep it clean.",
          link: "https://github.com/josephpcoyne/coyne.dev"
        },
        {
          name: "Vue RPG",
          bio:
            "A classic RPG game built with Vue.js during a speedrun development.",
          link: "https://github.com/josephpcoyne/vue-rpg"
        }
      ]
    };
  }
};
</script>

<style scoped>
</style>