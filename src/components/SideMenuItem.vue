<template>
  <div class="flex items-center w-full my-[20px]">
    <RouterLink
      :to="pageUrl"
      :class="
        pageUrl === route.path
          ? 'border-l-[#A02346] text-[#A02346]'
          : 'border-l-[#191911] text-[#fff]'
      "
      class="border-l-4 w-full hover:text-[#A02346]"
      @mouseenter="isHover()"
      @mouseleave="isHover()"
    >
      <div class="flex items-center pl-3 mx-3 cursor-pointer">
        <img :width="iconSize" :src="`/imgs/icons/${icon}.png`" />
        <div class="pl-3.5 font-[600] text-[17px]">{{ name }}</div>
      </div>
    </RouterLink>
  </div>
</template>
<script setup>
import { toRefs, ref, watchEffect } from "vue";
import { RouterLink, useRoute } from "vue-router";

const route = useRoute();

const props = defineProps({
  iconString: String,
  iconSize: Number,
  pageUrl: String,
  name: String,
});
const { iconString, pageUrl, name } = toRefs(props);

let icon = ref(null);

watchEffect(() => {
  if (route.path == pageUrl.value && icon.value === iconString.value + "-check")
    return;

  if (route.path == pageUrl.value) {
    icon.value = iconString.value + "-check";
  } else {
    icon.value = iconString.value + "-none";
  }
});

const isHover = () => {
  if (icon.value === iconString.value + "-check") {
    icon.value = iconString.value + "-none";
  } else if (icon.value === iconString.value + "-none") {
    icon.value = iconString.value + "-check";
  }
};
</script>
