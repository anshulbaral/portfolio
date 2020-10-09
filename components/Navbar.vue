<template>
  <div>
    <div class="border-r-2 bg-white h-screen">
      <div class="flex flex-wrap">
        <div class="flex flex-wrap bg-white py-2 px-4 shadow-xl rounded-lg">
          <h2 class="text-lg font-semibold text-teal-800 lg:text-2xl">Navigate</h2>
        </div>
      </div>
      <div class="h-full">
        <div class="mt-2 text-gray-600 text-lg font-semibold sm:text-sm md:text-lg lg:text-xl">
          <div class="flex items-center mb-2">
            <img class="h-6 mr-2 mt-1 mb-1" src="img/nav-icon.png" />
            <nuxt-link
              to="/about"
              class="px-2 py-1 rounded-md hover:text-gray-800 hover:shadow-lg"
            >About Us</nuxt-link>
          </div>
          <div class="flex items-center mb-2">
            <img class="h-6 mr-2 mt-1 mb-1" src="img/nav-icon.png" />
            <nuxt-link to="/" class="px-2 py-1 rounded-md hover:text-gray-800 hover:shadow-lg">Home</nuxt-link>
          </div>
          <div class="flex items-center mb-2">
            <img class="h-6 mr-2 mt-1 mb-1" src="img/nav-icon.png" />
            <nuxt-link
              to="/contact"
              class="px-2 py-1 rounded-md hover:text-gray-800 hover:shadow-lg"
            >Contact me</nuxt-link>
          </div>
          
        </div>
      </div>
    </div>
  </div>
</template>

<script>
</script>

<style>
</style>