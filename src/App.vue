<template>
  <div id="app" class="px-8 py-1 md:px-30 md:py-8 lg:px-40 lg:py-12 md:w-3/4 md:m-auto">
    <NavBar />
    
    <router-view />
  </div>
</template>
<script>
import NavBar from '@/components/NavBar.vue';

export default {
  components: {
    NavBar
  },
};
</script>
<style>
#app {
  font-family: Gilroy-Light;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  /* padding: 3rem 10rem; */
}
.font {
    font-family: Gilroy-ExtraBold;
}
</style>
