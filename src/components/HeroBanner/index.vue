<template>
  <div class="bg-[url('./src/assets/images/headerbg.gif')] w-full h-72 flex justify-center items-center">
    <img src="../../assets/images/logo.png" class=" w-72" />
  </div>
  <div class="pl-4 w-full h-20 bg-stone-950 flex justify-between items-center sticky top-0">
    <img src="../../assets/images/logo.png" class="w-20" />
    <div class="flex flex- gap-6">
      <label class="text-white">Twitter</label>
      <label class="text-white">Instagram</label>
      <label class="text-white">Listen</label>
    </div>
    <div>

    </div>
  </div>
</template>

<script setup>
  defineOptions({ name: 'hero-banner' })
</script>
