<script setup>
import Principal from './components/Principal.vue';
import Recorrido from './components/Recorrido.vue';
import Bloque from './components/Bloque.vue';
</script>

<template>
  <div class="container mt-4">
    <Principal />
    <div class="row">
      <div class="col-md-6">
        <Recorrido />
      </div>
      <div class="col-md-6">
        <Bloque />
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  background: linear-gradient(135deg, #1E3A8A, #3B82F6);
  padding: 20px;
  border-radius: 15px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
}
</style>
