<template>
  <div>
    <div class="h-full">
      <Header />

      <div class="flex">
        <Navbar v-if="x == true" class="sm:w-1/4 w-2/5" />

        <div class="w-full h-screen pl-3 pt-2 bg-gray-100">
          <div class="-ml-2">
            <button
              class="bg-teal-100 hover:bg-white text-blue-900 sh focus:outline-none hover:text-gray-800 rounded-full hover:shadow-lg"
              @click="x=!x"
            >
              <ChevronLeftIcon v-if="x == true" />
              <ChevronRightIcon v-else="x=!x" />
            </button>
          </div>
        </div>
      </div>
    </div>
    <div class="justify-end">
      <div
        class="flex flex-wrap p-2 hover:bg-gray-300 w-10 hover:shadow-xl focus:outline-none rounded-lg"
      >
        <button class>
          <nuxt-link to="/">
            <MailIcon />
          </nuxt-link>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
import {
  MenuIcon,
  MoreHorizontalIcon,
  ChevronRightIcon,
  ChevronLeftIcon,
  MailIcon,
} from "vue-feather-icons";

export default {
  components: {
    MenuIcon,
    MoreHorizontalIcon,
    ChevronRightIcon,
    ChevronLeftIcon,
    MailIcon,
  },
  data() {
    return {
      x: true,
      images: [
        {
          img: "/img/IMG_20200729_202423.jpg",
          description: "1st image details",
          show: false,
        },
        {
          img: "/img/IMG_20200729_202619.jpg",
          description: "2nd image details",
          show: false,
        },
        {
          img: "/img/IMG_20200729_202341.jpg",
          description: "3rd image details",
          show: false,
        },
        {
          img: "/img/IMG_20200729_202359.jpg",
          description: "4th image details",
          show: false,
        },
        {
          img: "/img/IMG_20200729_202347.jpg",
          description: "5th image details",
          show: false,
        },
        {
          img: "/img/IMG_20200729_202536.jpg",
          description: "6th image details",
          show: false,
        },
        {
          img: "/img/IMG_20200729_202608.jpg",
          description: "7th image details",
          show: false,
        },
        {
          img: "/img/IMG_20200729_202528.jpg",
          description: "8th image details",
          show: false,
        },
        {
          img: "/img/IMG_20200729_202450.jpg",
          description: "9th image details",
          show: false,
        },
      ],
    };
  },
};
</script>

<style>
</style>