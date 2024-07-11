<template>
  <div class="h-[25rem] w-full bg-red-700">
    <div class="bg-[url('./src/assets/images/terror2.png')] w-full h-full mix-blend-overlay opacity-50 flex justify-center items-center">
    </div>
    <div class="absolute h-[25rem] top-0 z-50 flex justify-center items-center w-full">
      <RotatingLogo />
    </div>
  </div>
  <div class="pl-4 w-full h-20 z-20 bg-stone-950 flex justify-center items-center sticky top-0">
    <img src="../../assets/images/logo.png" class="w-20 absolute left-5 hover:cursor-pointer hover:animate-spin-horizontal" alt = "Logo girando" />
    <div class="flex flex- gap-10 text-lg font-light">
      <a class="text-white hover:text-red-800 hover:cursor-pointer" target="_blank" :href="twitterUrl">T̙̞̤͕̟̞͕͓̙̙̗̩̎̍̔̿̔̚W̯̬̩͍̟͕̒̾̃̉̎͐̽̽͛̋ͅI͕͕͇̥͗́̆͑̒̏̈́͂̊̋͒T̥̠̙͍͇̫̰̐͆̓̾͋̄̓̂̏̓̃̓T̗͚͔͕̘̪͙͐͌̊͌̅̒͆E̝̙͚͙̘̱̤͙̯̱̦̞͛͋̀̌̂̇͒͊R͖̥̟͈̞̣̯̗̲̣̋̆̋̚</a>
      <a class="text-white hover:text-red-800 hover:cursor-pointer" target="_blank" :href="instagramUrl">I͔̖͉͈͚͖̱͚̖̗̿̆͌͐́̀̽̾̓Ǹ̙̥̮̤͇̬͒̄̌̅̽̄͊̓ͅS̱̭͚̦̗͈͚̀͗̐́̇͑͑̓͑̌̌T̠̟̯͓̪̭̗̠͙͎͈̀͌͗́̄̆A̬͕͕͇͋͆̉͒̊̏̉̑̐́̚̚G͈̙͙̮̑͑̽̈́͊́̽͒R͇̜̥̣̬̮̬̤͑̾̽̓͗͋̍̀̊ͅA͉͇͇̙̦͖̟͚̝̲̎͆̎͊M̱̩̙̱̥̥̐̐̆̑̾̈́̓͋͌ͅ</a>
      <a class="text-white hover:text-red-800 hover:cursor-pointer">L̤̬̮̯̗͕̠̣̓̾̽̃̽̓̏̊͗͊̑̓I̭̘̖̜̱̩͓͓̦̪̋́̍͗͗̌̈́̿̀̔̇̌S̝̱͈̩̅͆́̃̿͗͌̒̿Ṱ͉͇̘͍͐̋̆̒̔ͅĖ̦̖̖̪͈̠͓͎̦̪͍͌̔͗̾̉̓̊̆̈̅N̯͙͓̭̝̜̤̤̬͇͋͑̋̃̄̍͂̔̆̐̿ͅ</a>
    </div>
  </div>
</template>

<script setup>
  import RotatingLogo from '../RotatingLogo.vue'
  defineOptions({ name: 'hero-banner' })

  const twitterUrl = 'https://twitter.com/isotopxs'
  const instagramUrl = 'https://www.instagram.com/isotopxs/'
</script>
