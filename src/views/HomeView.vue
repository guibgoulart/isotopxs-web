<script setup>
import HeroBanner from '@/components/HeroBanner/index.vue'
import SpotifyListen from '@/components/SpotifyListen.vue'
</script>

<template>
  <div class="h-full w-full bg-red-900">
    <HeroBanner />
    <div
      class="w-full text-white noise-bg text-lg mix-blend-overlay opacity-10 z-50 h-screen"
    ></div>
    <div class="flex flex-col px-4 pt-5 gap-4 z-10 w-full h-full absolute top-[368px]">
      <SpotifyListen class="w-96"/>
    </div>
    <div
      class="w-full flex justify-center items-center text-white noise-bg text-lg mix-blend-overlay h-screen opacity-10"
    >
      content
    </div>
    <div
      class="w-full flex justify-center items-center text-white noise-bg text-lg mix-blend-overlay h-screen"
    >
      content
    </div>
    <div
      class="w-full flex justify-center items-center text-white noise-bg text-lg mix-blend-overlay h-screen"
    >
      content
    </div>
    <div
      class="w-full flex justify-center items-center text-white noise-bg text-lg mix-blend-overlay h-screen"
    >
      content
    </div>
  </div>
</template>

<style>
.noise-bg {
  background-image: url(https://i.imgur.com/W60mciV.gif);
}
</style>
