<template>
  <div class="mt-10 pt-12 md:mt-20 mx-6 px-6 md:mx-40">
    <div class="flex">
      <div class="float-left sm:w-full md:w-auto">
        <h2 class="text-2xl md:text-4xl w-full pb-4 font">Who am I?</h2>
        <p class="text-lg md:text-lg md:w-auto">
          My name is Joseph Coyne. I am a full-stack software developer. I am here to document my journey from my life as a business owner, to bartender, to software engineer.
          <br />
          <br />My aim for this site is to not only serve as a portfolio of sorts, but as a playground for testing new tech and features. It began as a test of TailwindCSS. You may recognize the inspiration. Currently I am working on making it serve as my own CMS.
          <br />
          <br />If you would like to know more or just want to say hi, feel free to
          <router-link class="text-blue-500 font-bold" to="contact">contact</router-link> me.
        </p>
      </div>
      <ProfileCard class="lg:w-full lg:float-right" />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
</style>
