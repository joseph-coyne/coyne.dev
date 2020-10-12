<template>
  <main class="flex flex-col mt-12 overflow-auto md:max-w-4xl mx-auto">
    <section class="pt-12 mt-2 md:py-16">
      <div class="container flex flex-col px-6">
        <h2 class="pb-4 font-semibold text-3xl  md:text-4xl">Contact</h2>
          <p class="text-lg md:text-lg">
            If you would like to reach me for any reason, feel free to email me:
            <span
              class="font-bold mail text-blue-800"
            ></span>
          </p>
         </div>
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
