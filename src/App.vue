<template>
  <div
    id="topNav"
    class="fixed w-[calc(100%-240px)] h-[56px] right-0 flex items-center justify-between border-b border-b-[#32323D]"
  >
    <div class="flex w-full items-center">
      <Magnify class="pl-6 pr-2 mt-1" fillColor="#7E7E7E" :size="22" />
      <input
        class="p-1 bg-transparent outline-none font-[300] placeholder-[#BEBEBE] text-[#fff] w-full max-w-xl"
        placeholder="Search"
        type="text"
      />
    </div>
    <div class="flex pr-10 items-center">
      <div class="mr-4 p-1 hover:bg-gray-600 rounded-full cursor-pointer">
        <Bell fillColor="#fff" :size="20" />
      </div>
      <img class="rounded-full w-[33px]" src="/imgs/avt.png" />
    </div>
  </div>

  <div
    id="sideNav"
    class="fixed w-[240px] bg-[#191911] h-[100vh] border-r border-r-[#32323D]"
  >
    <div class="w-full px-2 pt-3 cursor-pointer">
      <RouterLink to="/">
        <img src="/imgs/logo&text.png" />
      </RouterLink>
    </div>

    <div class="mt-[53px]"></div>

    <SideMenuItem iconString="music" :iconSize="20" pageUrl="/" name="Music" />

    <SideMenuItem
      iconString="explore"
      :iconSize="20"
      pageUrl="/artist"
      name="Explore"
    />
    <SideMenuItem
      iconString="favourite"
      :iconSize="20"
      pageUrl="/favourite"
      name="Favourites"
    />
  </div>

  <div
    id="main"
    class="fixed h-[calc(100%-56px)] w-[calc(100%-240px)] ml-[240px] mt-[56px] overflow-x-auto"
  >
    <RouterView />
  </div>

  <MusicPlayer v-if="currentTrack" />

  <SongLyrics
    v-if="isLyrics"
    :class="{
      'animate__animated animate__slideInUp animate__faster': isLyrics,
    }"
  />
</template>
<script setup>
import { onBeforeMount } from "vue";
import { RouterView, RouterLink } from "vue-router";

import Magnify from "vue-material-design-icons/Magnify.vue";
import Bell from "vue-material-design-icons/Bell.vue";
import SideMenuItem from "./components/SideMenuItem.vue";
import MusicPlayer from "./components/MusicPlayer.vue";
import SongLyrics from "./components/SongLyrics.vue";

import { useSongStore } from "./stores/listOfSongs";
import { storeToRefs } from "pinia";
const useSong = useSongStore();
const { isPlaying, currentTrack, isLyrics, trackTime } = storeToRefs(useSong);

onBeforeMount(() => {
  isPlaying.value = false;
  isLyrics.value = false;
  trackTime.value = "0:00";
});
</script>
