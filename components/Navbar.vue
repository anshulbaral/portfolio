<template>
  <div>
    <div class="border-r-2 bg-blue-900 h-screen">
      <div class="flex flex-wrap ml-2 text-xs underline mb-2">
        <div class="flex flex-wrap">
          <h2
            class="text-2xl font-semibold text-blue-400 sm:text-sm md:text-md lg:text-lg xl:text-2xl"
          >Navi</h2>
          <h2
            class="text-2xl font-semibold text-teal-200 sm:text-sm md:text-md lg:text-lg xl:text-2xl"
          >gate</h2>
        </div>
      </div>
      <div class="h-full">
        <div class="text-white text-sm font-semibold sm:text-sm lg:text-lg">
          <div class="flex items-center mb-2 hover:bg-blue-800">
            <img class="h-6 mr-2 mt-1 mb-1" src="img/nav-icon.png" />
            <nuxt-link to="/about" class="hover:bg-blue-800">About Us</nuxt-link>
          </div>
          <div class="flex items-center mb-2 hover:bg-blue-800">
            <img class="h-6 mr-2 mt-1 mb-1" src="img/nav-icon.png" />
            <nuxt-link to="/" class="hover:bg-blue-800">Home</nuxt-link>
          </div>
          <div class="flex items-center mb-2 hover:bg-blue-800">
            <img class="h-6 mr-2 mt-1 mb-1" src="img/nav-icon.png" />
            <nuxt-link to="/contact" class="hover:bg-blue-800">Contact me</nuxt-link>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>