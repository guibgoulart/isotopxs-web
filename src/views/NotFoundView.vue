<template>
  <div class="background h-screen w-screen">
    <!-- Foreground Content -->
    <div class="flex flex-col items-center justify-center h-full text-center relative">
      <!-- 404 Text on top of the gif -->
      <h1 class="absolute top-1/4 w-full text-6xl text-white font-papyrus">404</h1>
      <img src="../assets/images/spieker.gif" alt="Spieker Bebendo" class="w-1/2 mx-auto" />
      <h2 class="text-2xl mt-8 text-white">Ta perdido paizinho?</h2>
      <!-- Link to return to the home page -->
      <a href="/" class="mt-4 text-white">Volta pra home</a>
    </div>
  </div>
</template>

<style>
.background {
  background-image: url('../assets/images/palhaco.jpg');
  background-size: cover;
  background-repeat: repeat;
}
</style>
