<template>
  <div class="mt-10 pt-12 md:mt-20 mx-6 px-6 md:mx-40">
    <div class="flex">
      <div class="float-left sm:w-full">
        <h2 class="text-2xl md:text-4xl pb-4 font">Contact Me</h2>
        <p class="text-lg md:text-lg">
          If you would like to reach me for any reason, feel free to email me:
          <span
            class="font-bold mail"
          ></span>
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
.mail:before {
  content: "\006A\006F\0073\0065\0070\0068\0040\0063";
}
.mail:after {
  content: "\006F\0079\006E\0065\002E\0064\0065\0076";
}
</style>
