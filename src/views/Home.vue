<template>
  <main class="flex flex-col sm:mt-12 sm:max-w-4xl">
    <section class="pt-12">
      <div
        class="container flex flex-col sm:flex-row justify-between sm:items-center p-6 ">
        <div class="order-2 sm:order-1">
          <h1 class="text-2xl sm:text-4xl font-semibold leading-tight mb-6 ">
            Hello! I'm Joseph Coyne. 
            <br> I am a full stack developer.
          </h1>
          <p class="text-lg sm:text-xl text-gray-600 mb-8">
            Welcome to my website. Feel free to take a look around and
            <router-link class="text-indigo-500 hover:text-indigo-400 active:text-indigo-600 font-medium" to="contact">reach out</router-link> if you would like to connect. I am constantly looking for
            opportunities to grow and create and am happy to tackle any challenge.
          </p>
        </div>
        <div class="order-1 sm:order-2">
          <ProfileCard class=""/>
        </div>
      </div>
    </section>

    <div class="container flex flex-col px-6">
      <Projects />
    </div>
  </main>
</template>

<style scoped>
</style>

<script>
import ProfileCard from "@/components/ProfileCard.vue";
import Projects from "@/components/Projects.vue";
export default {
  name: "Home",
  components: {
    ProfileCard,
    Projects
  }
};
</script>
