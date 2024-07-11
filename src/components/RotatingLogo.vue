<template>
    <div 
      class="relative size-[450px] overflow-hidden perspective"
      ref="container"
    >
      <img 
        src="../assets/images/logo.png" 
        alt="Imagem" 
        class="absolute inset-0 w-full h-full object-cover transform transition-transform duration-300"
        :style="{ transform: `rotateX(0deg) rotateY(${rotateX}deg)` }"
      >
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        rotateX: 0,
        perspective: '1000px', // profundidade da perspectiva
        mouseX: 0,
        dampingFactor: 0.1 // fator de amortecimento
      };
    },
    mounted() {
      document.addEventListener('mousemove', this.handleMouseMove);
      requestAnimationFrame(this.updateRotation);
    },
    beforeUnmount() {
      document.removeEventListener('mousemove', this.handleMouseMove);
    },
    methods: {
      handleMouseMove(event) {
        this.mouseX = event.clientX;
      },
      updateRotation() {
        const container = this.$refs.container;
        if (!container) return;
  
        const { width, left } = container.getBoundingClientRect();
        
        // Calcula a posição relativa do mouse dentro do elemento
        const x = (this.mouseX - left) / width - 0.8;
  
        // Aplica o amortecimento ao valor de rotação no eixo X
        const targetRotateX = + 40 * x;
           
        this.rotateX += (targetRotateX - this.rotateX) * this.dampingFactor;
  
        // Atualiza a rotação da imagem
        requestAnimationFrame(this.updateRotation);
      }
    }
  };
  </script>
  
  <style scoped>
  .perspective {
    perspective: 1000px; /* Profundidade da perspectiva */
  }
  </style>
  