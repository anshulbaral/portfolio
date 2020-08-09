<template>
  <div>
    <div class="flex justify-between items-center p-2 sm:p-4 rounded-sm bg-teal-400">
      <img src="img/thinkingemoji.png" class="h-12 rounded-full" />
      <img class="rounded-lg shadow-lg h-16 sm:h-16 md:h-20 lg:h-24" src="img/heading.png" />
      <img src="img/thinkingemoji.png" class="h-6 rounded-full" />
    </div>
    <div>
      <div
        class="flex justify-center flex-wrap -mt-3 z-20 shadow-2xl sm:font-medium italic text-white bg-purple-400 rounded-md"
      >
        <div class="bg-indigo-700 p-2 rounded-full">A place where our talents meet.</div>
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