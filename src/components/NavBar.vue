<template>
  <div class="flex items-center justify-between">
    <div class="flex items-center">
      <router-link to="/" class="flex items-center">
        <img class="float-left h-12 w-12" src="../assets/logo.png" alt="Logo">
        <span class="hidden md:inline title text-xl">Joseph Coyne</span>
      </router-link>
    </div>

      <div class="flex justify-between">
        <router-link to="/about" class="text-center px-4 py-2 m-2">About</router-link> 
        <!-- <router-link to="/blog" class="text-center px-4 py-2 m-2">Blog</router-link>    -->
        <router-link to="/contact" class="text-center px-4 py-2 m-2">Contact</router-link>
      </div>
  </div>
</template>

<script>
  export default {
    name:"NavBar",
    
  }
</script>

<style scoped>
  .title {
    font-family: Gilroy-ExtraBold;
    text-decoration: none;
  } 
</style>