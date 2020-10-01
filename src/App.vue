<template>
  <div id="app">
    <!-- <div id="app" class="px-8 py-1 md:px-30 md:py-8 lg:px-30 lg:py-10 md:w-3/4 md:m-auto"> -->
    <NavBar class="inset-x-0 top-0 fixed" />

    <router-view />
  </div>
</template>
<script>
import NavBar from "@/components/NavBar.vue";

export default {
  components: {
    NavBar
  }
};
</script>
<style>
#app {
  font-family: -apple-system, BlinkMacSystemFont, Helvetica Neue, Roboto, Arial,
    Noto Sans, sans-serif, Apple Color Emoji, Segoe UI, Segoe UI Emoji,
    Segoe UI Symbol, Noto Color Emoji;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  /* padding: 3rem 10rem; */
}
.font {
  font-family: Gilroy-ExtraBold;
}
.font-medium {
  font-family: Gilroy-Medium;
}
</style>
