<template>
  <main class="mt-12 overflow-auto">
    <section class="pt-12 mt-2 md:py-16">
      <div class="container flex flex-col max-w-screen-md px-6 md:mx-auto">
        <h2 class="pb-4 font-semibold text-center text-3xl  md:text-4xl">Contact</h2>
          <p class="text-lg md:text-lg">
            If you would like to reach me for any reason, feel free to email me:
            <span
              class="font-bold mail"
            ></span>
          </p>
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
