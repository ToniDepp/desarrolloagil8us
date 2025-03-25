<script>
export default {
  data() {
    return {
      alumnos: [
        { nc: 21620095, nombre: 'Eduardo', carrera: 'ISC' },
        { nc: 21620008, nombre: 'Tomas', carrera: 'IM' },
        { nc: 21620010, nombre: 'Anthony', carrera: 'IC' },
        { nc: 21620027, nombre: 'Toni', carrera: 'ISC' },
        { nc: 21620003, nombre: 'Tomi', carrera: 'LAQ' }
      ]
    }
  }
}
</script>

<template>
  <div class="container mt-4">
    <h3 class="text-white mb-3">Lista de Estudiantes</h3>
    <div class="list-group">
      <div v-for="alumno in alumnos" :key="alumno.nc" class="list-group-item list-group-item-action" style="border-radius: 12px; background: #3D81D8; color: white; margin-bottom: 10px;">
        <strong class="text-light">{{ alumno.nc }}</strong>
        <p class="mb-1">{{ alumno.nombre }} - {{ alumno.carrera }}</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  background: linear-gradient(135deg, #1E40AF, #60A5FA);
  padding: 20px;
  border-radius: 12px;
}
h3 {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
</style>
