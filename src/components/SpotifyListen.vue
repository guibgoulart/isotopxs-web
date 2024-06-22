<template>
    <div class="rounded-t-xl">
      <header class="macbook-header bg-stone-950 py-2 px-4 flex items-center justify-between rounded-t-xl">
        <!-- Logo ou ícone -->
        <div class="flex items-center space-x-2">
          <span class="font-carrois-gothic font-bold text-white">Listen</span> <!-- Texto do título -->
        </div>
        <!-- Botões de controle (exemplo: minimizar, maximizar, fechar) -->
        <div class="flex space-x-2">
          <button class="w-4 h-4 bg-yellow-400 rounded-full"></button>
          <button class="w-4 h-4 bg-green-400 rounded-full"></button>
          <button class="w-4 h-4 bg-red-400 rounded-full"></button>
        </div>
      </header>
  
      <!-- Espaço para o conteúdo principal (iframe do Spotify) -->
      <div class="bg-[#a02020] rounded-b-2xl">
        <iframe style="border-radius: 12px;" src="https://open.spotify.com/embed/album/0tuW5KXw6JqPDL8UMrFGvQ?utm_source=generator" width="100%" height="352" frameborder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'MacbookHeader',
    // Componente Vue
  }
  </script>
  
  <style scoped>
  /* Estilo adicional para o cabeçalho */
  .macbook-header {
    border-bottom: 1px solid #222222; /* Linha inferior */
  }
  </style>
  