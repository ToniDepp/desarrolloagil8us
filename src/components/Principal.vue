<script setup>
import { ref } from 'vue';
const bienvenido = ref("Manejo de variables y v-for");
const nombre = ref("Eduardo Tomas");
const apellidos = ref("Feria Ortiz");
</script>

<template>
  <div class="card text-center shadow p-4 mb-4 rounded border-0 bg-gradient">
    <h2 class="text-light">{{ bienvenido }}</h2>
    <h5 class="text-white">{{ nombre }} {{ apellidos }}</h5>
  </div>
</template>

<style scoped>
.bg-gradient {
  background: linear-gradient(135deg, #1E40AF, #60A5FA);
  color: rgb(255, 255, 255);
  border-radius: 15px;
}
</style>

