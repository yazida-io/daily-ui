<template>
  <div class="bg-red-50 bg-opacity-80 min-h-screen">
    <div
        class="container mx-auto md:rounded-2xl p-4 bg-white text-center w-screen shadow-lg sticky md:top-2 bg-white z-10">
      <h1
          class="font-sans md:text-3xl text-2xl font-semibold text-center"
      >
        Welcome to Daily UI |
        <span class="bg-clip-text text-transparent bg-gradient-to-br from-gray-300 via-orange-500 to-orange-700">Yazida.io</span>
      </h1>
    </div>
    <main class="min-h-screen py-10">
      <section class="container mx-auto grid grid-cols-1 md:grid-cols-3 gap-4">

        <div
            v-for="({name, image, links}, index) in payload"
            :key="index"
            class="bg-white flex flex-col p-2 select-none rounded-xl overflow-hidden shadow-sm hover:shadow-xl transform hover:-translate-y-1 transition-all mx-4 md:mx-0"
        >
          <img :src="image" :alt="name" class="rounded-xl w-full max-h-[300px] h-full">
          <div class="flex justify-between items-center mt-4">
            <h3 class="font-bold text-warmGray-600">{{ name }}</h3>
            <div class="flex gap-2">
              <a
                  :href="links.template"
                  target="_blank"
                  class="bg-orange-200 bg-opacity-40 hover:bg-opacity-100 rounded-md p-2"
              >
                <svg style="width:24px;height:24px" viewBox="0 0 24 24">
                  <path fill="currentColor"
                        d="M17,22V20H20V17H22V20.5C22,20.89 21.84,21.24 21.54,21.54C21.24,21.84 20.89,22 20.5,22H17M7,22H3.5C3.11,22 2.76,21.84 2.46,21.54C2.16,21.24 2,20.89 2,20.5V17H4V20H7V22M17,2H20.5C20.89,2 21.24,2.16 21.54,2.46C21.84,2.76 22,3.11 22,3.5V7H20V4H17V2M7,2V4H4V7H2V3.5C2,3.11 2.16,2.76 2.46,2.46C2.76,2.16 3.11,2 3.5,2H7M13,17.25L17,14.95V10.36L13,12.66V17.25M12,10.92L16,8.63L12,6.28L8,8.63L12,10.92M7,14.95L11,17.25V12.66L7,10.36V14.95M18.23,7.59C18.73,7.91 19,8.34 19,8.91V15.23C19,15.8 18.73,16.23 18.23,16.55L12.75,19.73C12.25,20.05 11.75,20.05 11.25,19.73L5.77,16.55C5.27,16.23 5,15.8 5,15.23V8.91C5,8.34 5.27,7.91 5.77,7.59L11.25,4.41C11.5,4.28 11.75,4.22 12,4.22C12.25,4.22 12.5,4.28 12.75,4.41L18.23,7.59Z"/>
                </svg>
              </a>
              <a
                  :href="links.github"
                  target="_blank"
                  class="bg-blue-200 bg-opacity-40 hover:bg-opacity-100 rounded-md p-2"
              >
                <svg style="width:24px;height:24px" viewBox="0 0 24 24">
                  <path fill="currentColor"
                        d="M12,2A10,10 0 0,0 2,12C2,16.42 4.87,20.17 8.84,21.5C9.34,21.58 9.5,21.27 9.5,21C9.5,20.77 9.5,20.14 9.5,19.31C6.73,19.91 6.14,17.97 6.14,17.97C5.68,16.81 5.03,16.5 5.03,16.5C4.12,15.88 5.1,15.9 5.1,15.9C6.1,15.97 6.63,16.93 6.63,16.93C7.5,18.45 8.97,18 9.54,17.76C9.63,17.11 9.89,16.67 10.17,16.42C7.95,16.17 5.62,15.31 5.62,11.5C5.62,10.39 6,9.5 6.65,8.79C6.55,8.54 6.2,7.5 6.75,6.15C6.75,6.15 7.59,5.88 9.5,7.17C10.29,6.95 11.15,6.84 12,6.84C12.85,6.84 13.71,6.95 14.5,7.17C16.41,5.88 17.25,6.15 17.25,6.15C17.8,7.5 17.45,8.54 17.35,8.79C18,9.5 18.38,10.39 18.38,11.5C18.38,15.32 16.04,16.16 13.81,16.41C14.17,16.72 14.5,17.33 14.5,18.26C14.5,19.6 14.5,20.68 14.5,21C14.5,21.27 14.66,21.59 15.17,21.5C19.14,20.16 22,16.42 22,12A10,10 0 0,0 12,2Z"/>
                </svg>
              </a>
            </div>
          </div>
        </div>

      </section>
    </main>
  </div>
</template>

<script lang="ts">
import {defineComponent} from "vue";
import payload from "./payload.json"

export default defineComponent({
  name: "App",
  computed: {
    payload: () => payload
  }
});
</script>
