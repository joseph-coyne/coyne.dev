<template>
  <main class="font-sas flex flex-col mt-10 overflow-auto">
    <section class="pt-12 mt-2 md:py-16">
      <div class="container flex flex-col justify-between px-6 md:flex-row md:max-w-screen-lg md:items-center md:mx-auto">
        <div class="md:max-w-2xl order-2 md:order-1">
          <h2 class="text-2xl md:text-4xl pb-4 font">Contact Me</h2>
          <p class="text-lg md:text-lg">
            If you would like to reach me for any reason, feel free to email me:
            <span
              class="font-bold mail"
            ></span>
          </p>
         </div>
        </div>
      <ProfileCard class="lg:w-full lg:float-right" />
    </section>
  </main>
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
