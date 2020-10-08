<template>
  <main class="flex flex-col mt-12 overflow-auto ">
    <section class="pt-12 mt-2 md:py-16 ">
      <div
        class="container flex flex-col justify-between px-6 md:flex-row md:max-w-screen-lg md:items-center md:mx-auto"
      >
        <div class="md:max-w-2xl order-2 md:order-1">
          <h1 class="text-3xl font-semibold leading-tight md:text-5xl my-6 ">
            Hello!
            <br />I'm Joseph Coyne.
          </h1>
          <p class="text-lg md:text-xl text-gray-600 mb-8">
            Welcome to my website. Feel free to take a look around and
            <router-link class="text-blue-500 font-medium" to="contact">reach out</router-link> if you would like to connect. I am constantly looking for
            opportunities to grow and create and am happy to tackle any challenge.
          </p>
        </div>
        <div class="order-1 md:order-2">
          <ProfileCard class=""/>
        </div>
      </div>
    </section>

    <div class="container flex flex-col mx-auto overflow-auto md:max-w-screen-lg px-6">
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
