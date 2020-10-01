<template>
  <div class="mt-10 overflow-auto">
    <section class="md:block pt-12 mt-2 md:py-16">
      <div
        class="container flex flex-col md:flex-row justify-between md:items-center px-6 md:mx-40"
      >
        <div class="bio md:max-w-2xl order-2 md:order-1">
          <h1 class="text-3xl font font-bold md:text-5xl mb-8 leading-tight tracking-tight">
            Hello!
            <br />I'm Joseph Coyne.
          </h1>
          <p class="text-lg md:text-xl mb-8">
            Welcome to my website. Feel free to take a look around and
            <router-link class="text-blue-500 font-bold" to="contact">reach out</router-link> if you would like to connect. I am constantly looking for
            opportunities to grow and create and am happy to tackle any challenge.
          </p>
        </div>
        <div class="order-1 md:order-2 mb-8">
          <ProfileCard />
        </div>
      </div>
    </section>

    <div>
      <Projects class="my-16 md:mt-32" />
    </div>
  </div>
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
