<template>
  <header class="mb-10 bg-white">
    <div class="flex mx-2 p-2 md:px-40 my-2 max-w-full items-center justify-between">
      <router-link to="/" class="">
        <img class="hidden md:inline mb-2 h-12 w-12" src="../assets/logo.png" alt="Logo">
        <span class="title whitespace-no-wrap text-lg md:text-xl">Joseph Coyne</span>
      </router-link>
    
      <div @click="isOpen = !isOpen">
        <div v-if="!isOpen" class="h-1 flex md:hidden font-bold text-xl items-center">
          =
        </div>
        <div v-if="isOpen" class="md:hidden font-bold">
          X
        </div>
      </div>

  
      <div class="flex hidden md:inline justify-between">
        <router-link to="/about" class="text-center px-4 py-2 m-2">About</router-link> 
        <!-- <router-link to="/blog" class="text-center px-4 py-2 m-2">Blog</router-link>    -->
        <router-link to="/contact" class="text-center px-4 py-2 m-2">Contact</router-link>
      </div>
      </div>
      <div :class="isOpen ? 'block' : 'hidden'" class="md:hidden w-full absolute bg-white flex z-10">
        <router-link to="/about" class="text-center px-4 py-2 m-2">About</router-link> 
        <!-- <router-link to="/blog" class="text-center px-4 py-2 m-2">Blog</router-link>    -->
        <router-link to="/contact" class="text-center px-4 py-2 m-2">Contact</router-link>
      </div>
  </header>
</template>

<script>
  export default {
    name:"NavBar",
    data() {
      return {
        isOpen: false,
      }
    },
    
  }
</script>

<style scoped>
  .title {
    font-family: Gilroy-SemiBold;
    text-decoration: none;
  } 
</style>