<template>
  <div>
    <div
      class="flex justify-between items-center p-2 sm:p-4 rounded-sm bg-transparent"
    ><div>
      <img
        class="rounded-lg shadow-lg h-16 sm:h-16 md:h-20 lg:h-24"
        src="img/heading.png"
      /></div>
      
      <div class = "text-white font-semibold bg-purple-300 flex flex-wrap rounded-lg p-1">
        ALPHA
      </div>
    </div>
    <div>
      <div
        class="flex justify-center flex-wrap -mt-3 z-20 shadow-2xl sm:font-medium font-bold text-white bg-purple-400 rounded-lg "
      >
        NOTE : This website is still in development and many things are to be added and changed.
        <br>"The following components are temporary. And may not be there after website development is complete."
      </div>
    </div>
  </div>
</template>

<script>
import { MailIcon } from "vue-feather-icons";
export default {
  components: {
    MailIcon,
  },
};
</script>

<style>
</style>