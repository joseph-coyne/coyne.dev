<template>
  <header class="mb-10 bg-white">
    <div class="flex mx-2 px-3 md:px-40 max-w-full items-center justify-between overflow-visible">
      <router-link to="/" class="p-2">
        <img class="hidden md:inline mb-2 h-12 w-12" src="../assets/logo.png" alt="Logo" />
        <span class="title whitespace-no-wrap text-md md:text-xl font-bold">Joseph Coyne</span>
      </router-link>

      <div @click="isOpen = !isOpen" class="mobile md:hidden text-3xl inline-block items-center">
        <div v-if="!isOpen">=</div>
        <div v-if="isOpen">×</div>
      </div>

      <div class="hidden font-medium md:inline justify-between">
        <router-link to="/about" class="text-center px-4 py-2 m-2">About</router-link>
        <!-- <router-link to="/blog" class="text-center px-4 py-2 m-2">Blog</router-link>    -->
        <router-link to="/contact" class="text-center px-4 py-2 m-2">Contact</router-link>
      </div>
    </div>
    <div
      :class="isOpen ? 'block' : 'hidden'"
      class="md:hidden font-medium w-full absolute bg-blue-100 flex z-10"
    >
      <router-link to="/about"  class="text-center px-4 py-2 m-2"><span @click="close()">About</span></router-link>
      <!-- <router-link to="/blog" class="text-center px-4 py-2 m-2">Blog</router-link>    -->
      <router-link @click="close()" to="/contact"  class="text-center px-4 py-2 m-2"><span @click="close()">Contact</span></router-link>
    </div>
  </header>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      isOpen: false
    };
  },
  methods: {
    close() {
      this.isOpen = false;
  
    }
  }
};
</script>

<style scoped>
.title {
  font-family: Gilroy-SemiBold;
  text-decoration: none;
}
</style>