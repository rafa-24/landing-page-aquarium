<template>
    <section class="bg-primary text-white py-16">
      <div class="container mx-auto flex flex-col md:flex-row items-center justify-between px-6">
        <!-- Texto -->
        <div class="md:w-1/2 mb-8 md:mb-0">
          <h2 class="text-2xl md:text-3xl font-semibold mb-4">
            Impulsamos la innovación tecnológica de tu empresa con soluciones de software a medida.
          </h2>
          <p class="text-base md:text-lg mb-6">
            En Aquarium Devs, transformamos ideas en productos digitales excepcionales que optimizan procesos y generan resultados.
          </p>
          <p class="text-base md:text-lg mb-8">
            ¡Colabora con nosotros y lleva tu negocio al siguiente nivel!
          </p>
          <!-- Botón -->
          <button
            class="bg-white text-black font-semibold py-2 px-6 rounded-full shadow-md hover:bg-gray-100 transition duration-300"
          >
            Contáctenos
          </button>
        </div>

        <!-- Imagen -->
        <div class="md:w-1/2 flex justify-center">
          <img
            src="../public/banner-aquarium-devs.webp"
            alt="Aquarium Devs Collaboration"
            class="max-w-full h-auto"
          />
        </div>
      </div>
    </section>
  </template>

  <script setup>
  // Puedes importar una imagen desde tu carpeta de assets si necesitas
  // Por ejemplo: import illustration from '@/assets/illustration.png';
  </script>

  <style scoped>
  .bg-primary {
    background-color: #157690; /* Color personalizado */
  }
  </style>
