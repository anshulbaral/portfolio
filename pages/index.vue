<template>
  <div>
    <div class="h-full">
      <Header />

      <div class="flex">
        <Navbar v-if="x == true" class="sm:w-1/4 w-2/5" />

        <div class="w-full pl-3 pt-2 bg-gray-200">
          <div class="-ml-2">
            <button
              class="bg-teal-100 hover:bg-white text-blue-900 sh focus:outline-none hover:text-gray-800 rounded-full hover:shadow-lg"
              @click="x=!x"
            >
              <ChevronLeftIcon v-if="x == true" />
              <ChevronRightIcon v-else="x=!x" />
            </button>
          </div>
          <div class="mb-6">
            <div class="rounded-lg shadow-lg flex flex-wrap w-64 bg-white text-purple-600">
              <h1 class="text-3xl font-semibold ml-2">Portfolio</h1>
            </div>
            <div class="w-3/4 text-lg rounded-md font-semibold text-gray-900">
              <h2 class="ml-2">My best art works.</h2>
            </div>
          </div>
          <div class="flex flex-wrap items-start">
            <div
              v-for="i in images"
              class="rounded-lg w-48 h-44 shadow-lg bg-white mr-2 mb-2 text-center p-2"
            >
              <img class="rounded-lg" :src="i.img" alt />
              <button
                @click="i.show = !i.show"
                class="rounded-lg px-2 py-1 focus:outline-none hover:bg-gray-100 hover:shadow-lg"
              >
                <MoreHorizontalIcon />
              </button>
              <div v-if="i.show == true">{{ i.description }}</div>
            </div>
          </div>
          <div class="flex flex-wrap text-center">More coming soon...</div>
          <div>
            <div
              class="flex flex-wrap text-3xl font-semibold mt-4 rounded-lg px-2 shadow-lg w-64 bg-white text-purple-600"
            >Curious mind</div>

            <div
              class="text-md font-normal flex flex-wrap text-gray-800"
            >Invite your curious mind to the world of whys</div>
          </div>
        </div>
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
} from "vue-feather-icons";

export default {
  components: {
    MenuIcon,
    MoreHorizontalIcon,
    ChevronRightIcon,
    ChevronLeftIcon,
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

<style></style>
