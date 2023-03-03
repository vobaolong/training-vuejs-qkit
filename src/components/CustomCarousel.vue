<template>
  <div>
    <div class="flex justify-between pb-5 ml-8 mr-6">
      <RouterLink
        to="/artist"
        @mouseenter="isHoverCategory = true"
        @mouseleave="isHoverCategory = false"
        :class="isHoverCategory ? 'hover:text-[#A02346]' : 'text-white'"
        class="flex items-center cursor-pointer font-semibold text-xl"
      >
        {{ category }}
        <ChevronRight
          :fillColor="isHoverCategory ? '#A02346' : '#fff'"
          :size="25"
          class="mt-1"
        />
      </RouterLink>

      <div class="flex items-center">
        <button
          @click="slideTo(false)"
          class="rounded-full p-2 hover:bg-[#2b2b2b]"
        >
          <ChevronLeft fillColor="#fff" :size="30" />
        </button>
        <!--  -->
        <div class="px-2"></div>
        <button
          @click="slideTo(true)"
          class="rounded-full p-2 hover:bg-[#2b2b2b]"
        >
          <ChevronRight fillColor="#fff" :size="30" />
        </button>
      </div>
    </div>

    <Carousel
      class="mr-8"
      ref="carousel"
      v-model="currentSlide"
      :items-to-show="4"
      :items-to-scroll="4"
      :transition="800"
      snapAlign="start"
    >
      <Slide v-for="slide in data" :key="slide" class="flex items-baseline">
        <SliderItem :slide="slide" />
      </Slide>
    </Carousel>
  </div>
</template>

<script setup>
import { ref, toRefs } from "vue";
import { RouterLink } from "vue-router";
import ChevronLeft from "vue-material-design-icons/ChevronLeft.vue";
import ChevronRight from "vue-material-design-icons/ChevronRight.vue";
import "vue3-carousel/dist/carousel.css";
import { Carousel, Slide } from "vue3-carousel";
import SliderItem from "./SliderItem.vue";

const currentSlide = ref(0);
const isHoverCategory = ref(false);

const props = defineProps({
  category: String,
  data: Array,
});
const { data, category } = toRefs(props);

const slideTo = (value) => {
  if (value && currentSlide.value <= 7) {
    const res = currentSlide.value + 4;
    if (res <= 12) {
      currentSlide.value = currentSlide.value + 4;
    } else if (res > 12) {
      currentSlide.value = 12;
    }
  } else if (!value) {
    const res = currentSlide.value - 4;
    if (res > 0) {
      currentSlide.value = currentSlide.value - 4;
    } else if (res < 1) {
      currentSlide.value = 0;
    }
  }
};
</script>
