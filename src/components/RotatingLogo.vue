<template>
    <div 
      class="relative w-64 h-64 overflow-hidden perspective"
      ref="container"
    >
      <img 
        src="../assets/images/logo.png" 
        alt="Imagem" 
        class="absolute inset-0 w-full h-full object-cover transform transition-transform duration-300"
        :style="{ transform: `rotateX(${rotateX}deg) rotateY(${rotateY}deg)` }"
      >
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        rotateX: 0,
        rotateY: 0,
        perspective: '1000px', // profundidade da perspectiva
        mouseX: 0,
        mouseY: 0,
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
        this.mouseY = event.clientY;
      },
      updateRotation() {
        const container = this.$refs.container;
        if (!container) return;
  
        const { width, height, left, top } = container.getBoundingClientRect();
        
        // Calcula a posição relativa do mouse dentro do elemento
        const x = (this.mouseX - left) / width - 0.5;
        const y = (this.mouseY - top) / height - 0.5;
  
        // Aplica o amortecimento aos valores de rotação
        const targetRotateY = 50 * x;
        const targetRotateX = -50 * y;
  
        this.rotateY += (targetRotateY - this.rotateY) * this.dampingFactor;
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
  