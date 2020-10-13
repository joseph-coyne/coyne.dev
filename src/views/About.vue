<template>
  <main class="flex flex-col mt-12 md:max-w-4xl mx-auto">
    <section class="pt-12 mt-2 md:py-16">
      <div class="container flex flex-col px-6">
        <h2 class="pb-4 font-semibold text-3xl md:text-4xl">Who am I?</h2>
        <div class="flex flex-col text-lg">
          <p class="py-2 text-xl">
            My name is Joseph Coyne and I am a full-stack software developer. I am here after a journey that has led me through life as a business owner, to career bartender, to ultimately software engineer. 
          </p>
          <p>
            My pair programming navigator is Luna. She's not great at her job.
          </p>
          <img src="@/assets/images/luna.jpg" alt="Luna!" class="rounded-lg my-10">
            <p class="py-2">My aim for this site is to not only serve as a portfolio of sorts, but as a playground for testing new tech and features. It began as a test of TailwindCSS. I don't pride myself as a designer but I at least I can mold things to make them somewhat appealing. You may recognize the inspiration as I am attempting to learn by doing. </p>
            <p class="py-2"> Following that I am working on making this more of a central hub and a CMS of sorts. 
          </p>
          <p class="py-2">
            If you would like to know more about me or just want to say hi, feel free to
            <router-link
            class="text-blue-800 hover:text-blue-900 font-medium"
            to="contact">
              contact
            </router-link>
            me!
          </p>
        </div>
      </div>
        <!-- <ProfileCard class="lg:w-full lg:float-right" /> -->
    </section>
  </main>
</template>

<script>
export default {
  data() {
    return {
      imgMe: '@/assets/images/luna.jpg',
      imgLuna: '@/assets/images/luna.jpg'
    }
  },
};
</script>

<style scoped>
</style>
