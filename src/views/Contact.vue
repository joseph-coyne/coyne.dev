<template>
  <main class="flex flex-col mt-12 sm:max-w-4xl">
    <section class="pt-12 sm:mt-10 sm:py-16">
      <div class="container flex flex-col px-6">
        <h2 class="pb-4 font-semibold text-3xl sm:text-4xl">Contact</h2>
        <div class="flex flex-col text-lg">
          <p class="py-2 text-xl">
            If you would like to reach me for any reason, feel free to email me:
            <span
              class="font-bold mail text-blue-800"
            ></span>
          </p>
        </div>
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
