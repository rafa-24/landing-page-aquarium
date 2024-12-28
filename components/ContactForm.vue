<template>
  <form @submit.prevent="addProject()">
    <div class="grid gap-6 mb-6 md:grid-cols-2">
      <div>
        <label
          for="name"
          class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
          >Primer Nombre</label
        >
        <input
          v-model="body.firstName"
          type="text"
          id="name"
          class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
          placeholder="John"
          required
        />
      </div>
      <div>
        <label
          for="last_name"
          class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
          >Primer apellido</label
        >
        <input
          v-model="body.lastName"
          type="text"
          id="last_name"
          class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
          placeholder="Doe"
          required
        />
      </div>
      <div>
        <label
          for="company"
          class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
          >Nombre de empresa o negocio</label
        >
        <input
          v-model="body.companyName"
          type="text"
          id="company"
          class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
          placeholder="Flowbite"
          required
        />
      </div>
      <div>
        <label
          for="phone"
          class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
          >Telefono de contacto</label
        >
        <input
          v-model="body.phone"
          type="tel"
          id="phone"
          class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
          placeholder="123-45-678"
          required
        />
      </div>
      <div>
        <label
          for="country"
          class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
          >Pais</label
        >
        <input
          v-model="body.country"
          type="text"
          id="country"
          class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
          placeholder="Nombre de tu pais"
          required
        />
      </div>

      <div>
        <label
          for="email"
          class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
          >Email</label
        >
        <input
          v-model="body.email"
          type="email"
          id="email"
          class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
          placeholder="krys1234@gmail.com"
          required
        />
      </div>

      <div>
        <label
          for="description_project"
          class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
          >Idea de tu proyecto</label
        >
        <textarea
          v-model="body.descriptionProject"
          id="description_project"
          rows="4"
          class="block p-2.5 w-full text-sm text-gray-900 bg-gray-50 rounded-lg border border-gray-300 focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
          placeholder="Escribe tu idea aqui..."
        ></textarea>
      </div>
    </div>

    <button
      type="submit"
      class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm w-full sm:w-auto px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
    >
      Enviar
    </button>
  </form>
</template>

<script setup>
import { ref } from "vue";
import Swal from "sweetalert2";

const body = ref({
  firstName: "",
  lastName: "",
  companyName: "",
  phone: "",
  country: "",
  email: "",
  descriptionProject: "",
});

async function addProject() {
  try {
    console.log("Datos enviados", body.value);

    // Enviar datos al servidor
    const project = await fetch("http://localhost:9000/create/users", {
      method: "POST",
      headers: {
        "Content-Type": "application/json",
      },
      body: JSON.stringify(body.value),
    });

    const response = await project.json();

    if (response.status === 201 || response.error === false) {
      Swal.fire({
        title: "Éxito",
        text: "Nuestro equipo se pondra en contacto contigo",
        icon: "success",
        position: "top-end", // Coloca la alerta en la parte superior derecha
        showConfirmButton: false, // Opcional, oculta el botón de confirmación
        timer: 3000, // Opcional, cierra automáticamente después de 3 segundos
        toast: true, // Cambia el estilo de la alerta a tipo "toast"
      });
    }
  } catch (err) {
    console.error("Occurred error", err);
  }
}
</script>

<style lang="scss" scoped>
</style>