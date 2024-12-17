<template>
  <section class="bg-white py-12 px-6">
    <!-- Encabezado -->
    <div class="text-center mb-10">
      <h2 class="text-3xl font-bold mb-4">¿Que hacemos en aquarium Devs?</h2>
      <p class="text-gray-600 max-w-3xl mx-auto">
        En Aquarium Devs, convertimos tus ideas en soluciones digitales reales y
        efectivas. Co-creamos contigo, trabajando mano a mano para diseñar y
        desarrollar productos digitales innovadores, personalizados y de alto
        impacto que impulsan tu negocio al siguiente nivel. Nuestro enfoque
        combina creatividad, tecnología y estrategia para garantizar resultados
        excepcionales.
      </p>
    </div>

    <!-- Sección principal -->
    <div class="flex flex-col lg:flex-row items-center justify-between mb-12">
      <!-- Imagen -->
      <div class="w-full lg:w-1/2 flex justify-center mb-6 lg:mb-0">
        <img
          src="../public/aquariumDevs-muñecos-software.webp"
          alt="Software Illustration"
          class="max-w-full h-auto"
        />
      </div>
      <!-- Texto -->
      <div class="w-full lg:w-1/2 text-center lg:text-left">
        <h3 class="text-2xl font-bold mb-4">
          Desarrollo de software de vanguardia de principio a fin
        </h3>
        <h4 class="text-xl font-semibold mb-3">
          Eleve su negocio con soluciones inteligentes
        </h4>
        <p class="text-gray-600 leading-relaxed">
          Ofrecemos un desarrollo integral de productos digitales enriquecido
          con capacidades de IA. Nuestro enfoque basado en IA garantiza altos
          estándares y pruebas continuas para productos de alta calidad y fácil
          mantenimiento, desde la estrategia y el diseño del producto hasta el
          desarrollo front-end y back-end.
        </p>
      </div>
    </div>

    <!-- Sección de industrias -->
    <div>
      <h2 class="text-3xl font-bold text-center mb-6">
        Algunas de las industrias a las que prestamos servicios actualmente
      </h2>
      <div
        class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-6 justify-items-center text-center"
      >
        <!-- Tarjetas de industrias -->
        <div
          v-for="(industry, index) in industries"
          :key="index"
          class="flex flex-col items-center"
        >
          <img
            :src="industry.icon"
            :alt="industry.name"
            class="w-30 h-30 mb-3"
          />
          <p class="font-medium text-gray-700">{{ industry.name }}</p>
        </div>
      </div>
    </div>

    <!--Mensaje del ceo-->
    <div class="container mx-auto py-12 px-4">
      <h2 class="text-4xl font-bold text-center mb-8">
        Un mensaje de nuestro director ejecutivo
      </h2>

      <div class="flex items-center justify-center mb-12">
        <img
          class="w-20 h-30 p-1 rounded-full ring-2 ring-gray-300 dark:ring-gray-500"
          src="../public/foto-rafa.jpg"
          alt="Bordered avatar"
        />
      </div>

      <p class="text-lg text-gray-600 mb-6">
        En Aquarium Devs, entendemos que cada proyecto es único y representa más
        que una idea: es una visión de lo que tu empresa puede lograr. Nuestro
        compromiso es acompañarte en cada paso del camino, brindándote
        soluciones de software innovadoras y personalizadas que se alineen con
        tus objetivos. Nuestra prioridad es construir relaciones basadas en la
        confianza y la transparencia. Contamos con un equipo altamente
        capacitado y apasionado por transformar desafíos en oportunidades,
        garantizando calidad, seguridad y resultados tangibles.
      </p>

      <p class="text-lg text-gray-600 mb-6">
        Te invitamos a trabajar con nosotros y experimentar un enfoque
        colaborativo que llevará tu negocio al siguiente nivel. J untos, podemos
        crear soluciones que no solo cumplan con tus expectativas, sino que las
        superen. Estamos aquí para escuchar tus necesidades y convertir tus
        ideas en realidad.
      </p>
      <div class="flex justify-center">
        <p class="text-2xl font-bold mb-4">
            Rafael Prieto Ceo
        </p>
      </div>
    </div>
  </section>
</template>

  <script setup>
import educationalIcon from "@/public/industria-educativa.webp";
import financialIcon from "@/public/tecnologia-financiera.webp";
import medicalIcon from "@/public/Tecnologia-medica.webp";
import highTechIcon from "@/public/industria-alta-tecnologia.webp";
import retailIcon from "@/public/industria-minorista.webp";
import iotIcon from "@/public/industria-iot.webp";

// Lista de industrias
const industries = [
  { name: "Tecnología Educativa", icon: educationalIcon },
  { name: "Tecnología financiera", icon: financialIcon },
  { name: "Tecnología médica", icon: medicalIcon },
  { name: "De alta tecnología", icon: highTechIcon },
  { name: "Minorista", icon: retailIcon },
  { name: "IOT", icon: iotIcon },
];
</script>

  <style scoped>
/* Puedes agregar estilos personalizados si es necesario */
</style>
