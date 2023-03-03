<template>
  <RouterLink to="/artist" class="cursor-pointer">
    <div
      class="relative"
      @mouseenter="isHover = true"
      @mouseleave="isHover = false"
    >
      <div
        :class="
          isHover
            ? 'transition ease-in bg-opacity-30 duration-150'
            : 'transition ease-out bg-opacity-5 duration-150'
        "
        class="w-full h-full z-10 bg-black rounded-md absolute"
      />
      <div class="pl-4 pt-4 absolute z-50">
        <div
          class="max-w-md inline-blocktext-white px-2 py-1 text-sm text-white text-center rounded-md bg-black bg-opacity-40"
        >
          Album
        </div>
        <div class="text-rose-100 text-xl mt-2 font-[700]">{{ by }}</div>
        <div class="text-rose-100 mt-2 font-[400]">{{ song }}</div>
      </div>
      <div class="absolute z-50 bottom-3 left-3 rounded-full bg-white p-1.5">
        <Play :size="27" />
      </div>
      <img class="rounded-lg" :src="image" />
    </div>
  </RouterLink>
</template>

<script setup>
import { ref } from "vue";
import { RouterLink } from "vue-router";
import Play from "vue-material-design-icons/Play.vue";
let isHover = ref(false);
const props = defineProps({ by: String, song: String, image: String });
</script>
