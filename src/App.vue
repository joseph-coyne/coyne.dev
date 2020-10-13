<template>
  <div id="app"
  class="h-screen overflow-auto"
   :class="[ currentRoute ? 'bg-blue-800' : 'bg-white' ]">

    <NavBar class="inset-x-0 top-0 fixed" />

    <router-view/>
  </div>
</template>
<script>
import NavBar from "@/components/NavBar.vue";

export default {
  components: {
    NavBar
  },
  computed: {
    currentRoute() {
      return this.$route.name === 'Login' || this.$route.name === 'Admin'
    }
  },
};
</script>
<style>

</style>
