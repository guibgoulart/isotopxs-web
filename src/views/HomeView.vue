<script setup>
  import HeroBanner from '@/components/HeroBanner/index.vue'
</script>

<template>
  <div class=" h-full w-full bg-red-950 ">
    <HeroBanner />
    <div class="w-full text-white noise-bg text-lg mix-blend-overlay Z-50 h-screen">
    </div>
    <div class="flex justify-center items-center z-10 w-full h-full absolute top-0">
      <span class="text-white text-6xl">
        CONTEUDO
      </span>
    </div>
    <div class="w-full flex justify-center items-center text-white noise-bg text-lg mix-blend-overlay h-screen">
      content
    </div>
    <div class="w-full flex justify-center items-center text-white noise-bg text-lg mix-blend-overlay h-screen">
      content
    </div>
    <div class="w-full flex justify-center items-center text-white noise-bg text-lg mix-blend-overlay h-screen">
      content
    </div>
    <div class="w-full flex justify-center items-center text-white noise-bg text-lg mix-blend-overlay h-screen">
      content
    </div>
  </div>
</template>

<style>
.noise-bg {
    background-image: url(https://i.imgur.com/W60mciV.gif);
}
</style>