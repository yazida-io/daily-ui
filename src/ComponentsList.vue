<template>
  <section class="container mx-auto grid grid-cols-1 md:grid-cols-3 gap-4">
    <div
        v-for="({name, image, links}, index) in payload"
        :key="index"
        class="bg-white flex flex-col p-2 select-none rounded-xl overflow-hidden shadow-sm hover:shadow-xl transform hover:-translate-y-1 transition-all mx-4 md:mx-0"
    >
      <component-card :image="image" :links="links" :name="name"/>
    </div>

  </section>
</template>
<script lang="ts">
import ComponentCard from "./ComponentCard.vue"
import payload from "./payload.json";

export default {
  name: 'ComponentsList',
  components: {ComponentCard},
  computed: {
    payload: () => payload
  }
}
</script>
