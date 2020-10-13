<template>
  <main class="flex flex-col mt-12 md:max-w-4xl mx-auto">
    <section class="pt-12 mt-2 md:py-16">
      <div class="flex justify-center">
        <form @submit.prevent class="flex flex-col justify-center rounded w-1/2">
        <div class="flex flex-col p-12  w-full bg-white rounded-t text-center">
          <p class="text-lg">Looks like you found my admin page!</p>
          <p class="text-gray-600 my-4">Would you like to see what it looks like?</p>
          <button
            class="bg-indigo-600 hover:bg-indigo-500 active:bg-indigo-700 place-self-center font-open font-semibold text-sm text-white rounded py-2 px-4 w-24 shadow-md transform ease-in-out active:outline-none focus:outline-none duration-200 hover:-translate-y-0.5 "
          >DEMO
          </button>
        </div>
          <div class="flex flex-col p-12 w-full bg-gray-200 rounded-b">
            <div class="relative flex flex-wrap items-stretch mb-5">
              <span class="z-10 h-full leading-snug font-normal text-center text-gray-400 absolute bg-transparent rounded text-open items-center justify-center w-8 pl-2 py-2">
                <i class="fas fa-envelope"></i>
              </span>
              <input type="email" placeholder="Email" class="p-2 placeholder-gray-400 text-gray-700 relative bg-white rounded text-sm shadow outline-none focus:outline-none w-full pl-10"/>
            </div>
            <div class="relative flex flex-wrap items-stretch mb-3">
              <span class="z-10 h-full leading-snug font-normal text-center text-gray-400 absolute bg-transparent rounded text-open items-center justify-center w-8 pl-2 py-2">
                <i class="fas fa-lock"></i>
              </span>
              <input type="password" placeholder="Password" class="p-2 placeholder-gray-400 text-gray-700 relative bg-white rounded text-sm shadow outline-none focus:outline-none w-full pl-10"/>
            </div>
            <div class="relative">
              <input type="checkbox" class="z-10 appearance-none cursor-pointer rounded p-2 my-2 mr-2 bg-white shadow checked:bg-blue-900 checked:border-transparent "> 
              <i class="fas fa-check text-white text-2xs checked:hidden absolute pointer-events-none ml-.75 left-0 top-sm"></i>
              <span class="text-gray-600 absolute pt-1">Remember Me</span>
            </div>
            <router-link to="/admin"
              class="bg-indigo-600 text-center place-self-center hover:bg-blue-900 font-open font-semibold text-sm text-white rounded py-2 px-4 w-24 mt-8 shadow-md transform ease-in-out active:outline-none focus:outline-none duration-200 hover:-translate-y-0.5 ">
              SIGN IN
            </router-link>
          </div>
          
        </form>
      </div>
    </section>
  </main>
</template>

<script>
  export default {
    name:"Login"
    
  }
</script>

<style>

</style>