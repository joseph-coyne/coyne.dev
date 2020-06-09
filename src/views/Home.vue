<template>
  <div class="mt-6 md:mt-32">
    <div class="flex">
      <div class="float-left sm:w-full">
        <h2 class="text-4xl md:text-5xl w-full pb-4">Hello, I'm Joseph</h2>
        <p class="text-lg md:text-2xl md:w-4/5">I'm a full-stack software developer constantly looking for opportunities to grow and create.</p>
      </div>
        <ProfileCard class="md:float-right"/>
    </div>
    <div>
      <Projects class="mt-32" />
    </div>
  </div>
</template>

<style scoped>
h2{
  font-family: Gilroy-ExtraBold;
}
</style>

<script>
import ProfileCard from '@/components/ProfileCard.vue';
import Projects from '@/components/Projects.vue';
export default {
  name: "Home",
  components: {
    ProfileCard,
    Projects
  }
};
</script>
