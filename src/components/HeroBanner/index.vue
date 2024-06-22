<template>
  <div class="bg-[url('./src/assets/images/headerbg.gif')] w-full h-72 flex justify-center items-center">
    <RotatingLogo class="absolute"/>
  </div>
  <div class="pl-4 w-full h-20 z-20 bg-stone-950 flex justify-center items-center sticky top-0">
    <img src="../../assets/images/logo.png" class="w-20 absolute left-5 hover:cursor-pointer hover:animate-spin-horizontal" />
    <div class="flex flex- gap-6">
      <a class="text-white hover:text-red-800 hover:cursor-pointer font-carrois-gothic" target="_blank" :href="twitterUrl">Twitter</a>
      <a class="text-white hover:text-red-800 hover:cursor-pointer" target="_blank" :href="instagramUrl">Instagram</a>
      <a class="text-white hover:text-red-800 hover:cursor-pointer">Listen</a>
    </div>
  </div>
</template>

<script setup>
  import RotatingLogo from '../RotatingLogo.vue'
  defineOptions({ name: 'hero-banner' })

  const twitterUrl = 'https://twitter.com/isotopxs'
  const instagramUrl = 'https://www.instagram.com/isotopxs/'
</script>
