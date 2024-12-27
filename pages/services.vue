<template>
  <div>
    <NavBar />
    <DescriptionHome />
    <section class="bg-white py-12 px-6">
      <!-- Encabezado -->
      <div class="text-center mb-10">
        <h2 class="text-3xl font-bold mb-4">¿Por qué AquariumDevs?</h2>
        <p class="text-gray-600 max-w-3xl mx-auto">
          En AquariumDevs creamos soluciones digitales personalizadas que se
          adaptan a las necesidades específicas de tu negocio. Nuestro equipo
          combina experiencia, innovación y un alto estándar de calidad para
          garantizar resultados confiables y efectivos. Contáctanos para llevar
          tu proyecto al siguiente nivel.
        </p>
      </div>
    </section>
    <div class="container mx-auto px-4 py-8">
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8 text-center">
        <!-- Card 1 -->
        <div
          class="flex flex-col items-center bg-white p-6 rounded-lg shadow-md hover:shadow-lg"
        >
          <div class="mb-4">
            <!-- Icon -->
            <img
              src="../public/soluciones-para-empresas.svg"
              alt="soluciones para empresas"
              class="h-16 w-16"
            />
          </div>
          <h3 class="text-lg font-bold mb-2">
            Soluciones para Empresas y Startups
          </h3>
          <p class="text-sm text-gray-600 mb-4">
            Nuestro equipo trabaja integrado con sus equipos, bajo nuestra
            gestión experta. Seleccionamos el mejor talento posible para sus
            necesidades y gestionamos el equipo para maximizar los resultados de
            su proyecto.
          </p>
        </div>

        <!-- Card 2 -->
        <div
          class="flex flex-col items-center bg-white p-6 rounded-lg shadow-md hover:shadow-lg"
        >
          <div class="mb-4">
            <!-- Icon -->
            <img
              src="../public/soluciones-para-empresas.svg"
              alt="Icono 2"
              class="h-16 w-16"
            />
          </div>
          <h3 class="text-lg font-bold mb-2">
            Desarrollo de aplicaciones web y móviles
          </h3>
          <p class="text-sm text-gray-600 mb-4">
            Nuestro equipo trabaja integrado con sus equipos, bajo nuestra
            gestión experta. Seleccionamos el mejor talento posible para sus
            necesidades y gestionamos el equipo para maximizar los resultados de
            su proyecto.
          </p>
        </div>

        <!-- Card 3 -->
        <div
          class="flex flex-col items-center bg-white p-6 rounded-lg shadow-md hover:shadow-lg"
        >
          <div class="mb-4">
            <!-- Icon -->
            <img
              src="../public/diseño-de-productos.svg"
              alt="Icono 3"
              class="h-16 w-16"
            />
          </div>
          <h3 class="text-lg font-bold mb-2">Diseño de producto</h3>
          <p class="text-sm text-gray-600 mb-4">
            Nuestro equipo trabaja integrado con sus equipos, bajo nuestra
            gestión experta. Seleccionamos el mejor talento posible para sus
            necesidades y gestionamos el equipo para maximizar los resultados de
            su proyecto.
          </p>
        </div>
      </div>
    </div>

    <!-- Areas de desarrollo de software -->
    <section class="bg-white py-12 px-6">
      <!-- Encabezado -->
      <div class="text-center mb-10">
        <h2 class="text-3xl font-bold mb-4">
          Desarrollo de software personalizado
        </h2>

        <!-- iconos areas de software -->
        <div class="container mx-auto px-4 py-8">
          <div class="grid grid-cols-1 md:grid-cols-3 gap-8 text-center">
            <!-- diseño ux ui -->
            <div
              class="flex flex-col items-center bg-white p-6 rounded-lg shadow-md hover:shadow-lg"
            >
              <div class="mb-4">
                <!-- Icon -->
                <img
                  src="../public/ux-ux-design-careers.svg"
                  alt="soluciones para empresas"
                  class="h-16 w-16"
                />
              </div>
              <h3 class="text-lg font-bold mb-2">
                Diseño UX/UI
              </h3>
              <p class="text-sm text-gray-600 mb-4">
                El viaje comienza con nuestro equipo de diseño UX/UI. Ellos tomaran tu idea de software y la convertiran en bocetos y prototipos visuales.
              </p>
            </div>

            <!-- desarrollo mobile -->
            <div
              class="flex flex-col items-center bg-white p-6 rounded-lg shadow-md hover:shadow-lg"
            >
              <div class="mb-4">
                <!-- Icon -->
                <img
                  src="../public/mobile-development-careers.svg"
                  alt="Icono 2"
                  class="h-16 w-16"
                />
              </div>
              <h3 class="text-lg font-bold mb-2">
                Desarrollo de aplicaciones móviles
              </h3>
              <p class="text-sm text-gray-600 mb-4">
                Con el diseño en mano, nuestro equipo de desarrollo de aplicaciones móviles comenzara a trabajar.
              </p>
            </div>

            <!-- project manager -->
            <div
              class="flex flex-col items-center bg-white p-6 rounded-lg shadow-md hover:shadow-lg"
            >
              <div class="mb-4">
                <!-- Icon -->
                <img
                  src="../public/project-management-careers.svg"
                  alt="Icono 3"
                  class="h-16 w-16"
                />
              </div>
              <h3 class="text-lg font-bold mb-2">Project manager</h3>
              <p class="text-sm text-gray-600 mb-4">
                Mientras el equipo trabajaba, nuestro Project Manager esta al mando, asegurándose de que todo marchara según el plan.
              </p>
            </div>

            <!-- devops -->
            <div
              class="flex flex-col items-center bg-white p-6 rounded-lg shadow-md hover:shadow-lg"
            >
              <div class="mb-4">
                <!-- Icon -->
                <img
                  src="../public/devops-careers.svg"
                  alt="Icono 3"
                  class="h-16 w-16"
                />
              </div>
              <h3 class="text-lg font-bold mb-2">DevOps</h3>
              <p class="text-sm text-gray-600 mb-4">
                A medida que el proyecto avanzaba, nuestro equipo de DevOps entra en acción para garantizar que la plataforma sea segura, estable y escalable.
              </p>
            </div>

            <!-- Desarrollo frontend -->
            <div
              class="flex flex-col items-center bg-white p-6 rounded-lg shadow-md hover:shadow-lg"
            >
              <div class="mb-4">
                <!-- Icon -->
                <img
                  src="../public/frontend-development-careers.svg"
                  alt="Icono 3"
                  class="h-16 w-16"
                />
              </div>
              <h3 class="text-lg font-bold mb-2">Desarrollo frontend</h3>
              <p class="text-sm text-gray-600 mb-4">
                El siguiente paso es llevado a cabo por el equipo de desarrollo frontend, quienes dieron vida a los diseños creados por UX/UI.
              </p>
            </div>


            <!-- Desarrollo backend -->
            <div
              class="flex flex-col items-center bg-white p-6 rounded-lg shadow-md hover:shadow-lg"
            >
              <div class="mb-4">
                <!-- Icon -->
                <img
                  src="../public/backend-development-careers.svg"
                  alt="Icono 3"
                  class="h-16 w-16"
                />
              </div>
              <h3 class="text-lg font-bold mb-2">Desarrollo backend</h3>
              <p class="text-sm text-gray-600 mb-4">
                Por último, nuestro equipo de desarrollo backend se encargó de construir el motor que hara funcionar toda tu plataforma.
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Ideas de proyectos -->
    <section class="bg-white py-12 px-6">
      <!-- Encabezado -->
      <div class="text-center mb-10">
        <h2 class="text-3xl font-bold mb-4">¿Tienes un proyecto en mente? Compartelo con nosotros</h2>
      </div>
      <ContactForm/>
    </section>
    <Footer/>
  </div>
</template>

<script setup>
</script>

<style lang="scss" scoped>
</style>