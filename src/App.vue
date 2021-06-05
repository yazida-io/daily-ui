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
      <ComponentsList/>
    </main>
  </div>
</template>

<script lang="ts">
import {defineComponent} from "vue";
import ComponentsList from "./ComponentsList.vue";
import SignIn from "./components/001/SignIn.vue";

export default defineComponent({
  name: "App",
  components: {SignIn, ComponentsList},
});
</script>
