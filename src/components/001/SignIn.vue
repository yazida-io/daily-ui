<template>
  <div class="bg-warmGray-200 h-screen fixed top-0 left-0 w-screen z-30 overflow-hidden">
    <div class="relative h-full w-full top-0 left-0">
      <div
          class="w-[1200px] mx-auto absolute top-20 left-1/2 transform -translate-x-1/2 h-[700px] rounded-xl grid grid-cols-1 md:grid-cols-12 shadow-lg bg-white overflow-hidden">

        <!-- -->
        <div class="col-span-6 p-4 relative">
          <div
              class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-1/2 space-y-10 text-center"
          >
            <h1 class="text-4xl text-[#004156] font-bold">
              Welcome back !
            </h1>

            <div class="flex gap-4 justify-center items-center">
              <!-- Google -->
              <button class="w-10 h-10 bg-[#dd4b39] rounded-full p-2">
                <svg viewBox="0 0 24 24">
                  <path fill="white"
                        d="M23,11H21V9H19V11H17V13H19V15H21V13H23M8,11V13.4H12C11.8,14.4 10.8,16.4 8,16.4C5.6,16.4 3.7,14.4 3.7,12C3.7,9.6 5.6,7.6 8,7.6C9.4,7.6 10.3,8.2 10.8,8.7L12.7,6.9C11.5,5.7 9.9,5 8,5C4.1,5 1,8.1 1,12C1,15.9 4.1,19 8,19C12,19 14.7,16.2 14.7,12.2C14.7,11.7 14.7,11.4 14.6,11H8Z"/>
                </svg>
              </button>

              <!-- Facebook -->
              <button class="w-10 h-10 bg-[#3b5999] rounded-full p-2 text-white">
                <svg viewBox="0 0 24 24">
                  <path fill="white"
                        d="M12 2.04C6.5 2.04 2 6.53 2 12.06C2 17.06 5.66 21.21 10.44 21.96V14.96H7.9V12.06H10.44V9.85C10.44 7.34 11.93 5.96 14.22 5.96C15.31 5.96 16.45 6.15 16.45 6.15V8.62H15.19C13.95 8.62 13.56 9.39 13.56 10.18V12.06H16.34L15.89 14.96H13.56V21.96A10 10 0 0 0 22 12.06C22 6.53 17.5 2.04 12 2.04Z"/>
                </svg>
              </button>

              <!-- LinkedIn -->
              <button class="w-10 h-10 bg-[#0077B5] rounded-full p-2">
                <svg viewBox="0 0 24 24">
                  <path fill="white"
                        d="M19 3A2 2 0 0 1 21 5V19A2 2 0 0 1 19 21H5A2 2 0 0 1 3 19V5A2 2 0 0 1 5 3H19M18.5 18.5V13.2A3.26 3.26 0 0 0 15.24 9.94C14.39 9.94 13.4 10.46 12.92 11.24V10.13H10.13V18.5H12.92V13.57C12.92 12.8 13.54 12.17 14.31 12.17A1.4 1.4 0 0 1 15.71 13.57V18.5H18.5M6.88 8.56A1.68 1.68 0 0 0 8.56 6.88C8.56 5.95 7.81 5.19 6.88 5.19A1.69 1.69 0 0 0 5.19 6.88C5.19 7.81 5.95 8.56 6.88 8.56M8.27 18.5V10.13H5.5V18.5H8.27Z"/>
                </svg>
              </button>
            </div>

            <p class="text-warmGray-400">
              Or use your email account
            </p>

            <form action="#" class="space-y-3">
              <label for="email" class="flex items-center gap-2 bg-warmGray-100 px-2 rounded-md">
                <svg class="w-6 h-6" viewBox="0 0 24 24">
                  <path fill="#AAA"
                        d="M20,8L12,13L4,8V6L12,11L20,6M20,4H4C2.89,4 2,4.89 2,6V18A2,2 0 0,0 4,20H20A2,2 0 0,0 22,18V6C22,4.89 21.1,4 20,4Z"/>
                </svg>
                <input class="focus:outline-none flex-1 bg-transparent py-3 px-2" id="email" type="email"
                       placeholder="Email">
              </label>

              <label for="password" class="flex items-center gap-2 bg-warmGray-100 px-2 rounded-md">
                <svg class="w-6 h-6" viewBox="0 0 24 24">
                  <path fill="#AAA"
                        d="M12,17A2,2 0 0,0 14,15C14,13.89 13.1,13 12,13A2,2 0 0,0 10,15A2,2 0 0,0 12,17M18,8A2,2 0 0,1 20,10V20A2,2 0 0,1 18,22H6A2,2 0 0,1 4,20V10C4,8.89 4.9,8 6,8H7V6A5,5 0 0,1 12,1A5,5 0 0,1 17,6V8H18M12,3A3,3 0 0,0 9,6V8H15V6A3,3 0 0,0 12,3Z"/>
                </svg>

                <input class="focus:outline-none flex-1 bg-transparent py-3 px-2" id="password" type="password"
                       placeholder="Password">
              </label>

              <p class="text-center">
                <a href="#" class="underline text-warmGray-400 hover:text-warmGray-500">
                  forgot password ?
                </a>
              </p>

              <button
                  class="uppercase text-red-50 bg-[#004156] py-3 px-10 rounded-full select-none focus:outline-none transform hover:-translate-y-1 transition">
                Sign In
              </button>
            </form>
          </div>
        </div>

        <!-- -->
        <div class="col-span-6 p-4 bg-[#004156] relative">
          <div
              class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 text-white w-1/2 space-y-10 text-center"
          >
            <h2 class="text-3xl text-white font-bold">
              New here ? <br/> Create your account
            </h2>
            <p class="text-lg text-white font-thin">
              Enter your personal details <br/> and start the journey with us
            </p>
            <button
                class="uppercase text-white border border-white py-3 px-10 rounded-full select-none focus:outline-none">
              Sign Up
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import {defineComponent} from "vue";

export default defineComponent({
  name: "SignIn",
  data: () => ({}),
})
</script>
