<template>
  <div class="">
      <section class="flex block py-16">
        <div class="flex flex-row justify-between items-center px-8 mx-40">
          <div class="bio max-w-2xl">
            <h1 class="text-4xl font-bold md:text-5xl mb-8">Hello, I'm Joseph Coyne.</h1>
            <p class="text-lg md:text-xl mb-8">
              This is my site to show off that I'm a full-stack software developer. I am constantly looking for
              opportunities to grow and create and will be happy to tackle any challenge.
            </p>
          </div>
          <div class="">
           <ProfileCard />
          </div>
        </div>
      </section>

    <div>
      <Projects class="mt-32" />
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
