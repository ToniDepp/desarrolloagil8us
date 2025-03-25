<script>
export default {
  data() {
    return {
      canciones: [
        { ISRC: 'CC-212-YY-84321', grupo: 'Radiohead', cancion: 'Karma Police', album: 'OK Computer' },
        { ISRC: 'CC-014-YY-91783', grupo: 'The Strokes', cancion: 'Reptilia', album: 'Room On Fire' },
        { ISRC: 'CC-792-YY-42108', grupo: 'Pink Floyd', cancion: 'Take it Back', album: 'The Division Bell' },
        { ISRC: 'CC-102-YY-09308', grupo: 'The Beatles', cancion: 'Happiness is a warm gun', album: 'White Album' },
        { ISRC: 'CC-981-YY-10120', grupo: 'The Strokes', cancion: 'Vision Of Division', album: 'First Impressions of Earth' }
      ]
    }
  }
}
</script>

<template>
  <div class="container mt-4">
    <h3 class="text-white mb-3">Lista de Canciones</h3>
    <div class="list-group">
      <div v-for="cancionx in canciones" :key="cancionx.ISRC" class="list-group-item list-group-item-action" style="border-radius: 12px; background: #3D81D8; color: white; margin-bottom: 10px;">
        <strong class="text-light">{{ cancionx.ISRC }}</strong>
        <p class="mb-1">{{ cancionx.grupo }} - {{ cancionx.cancion }} ({{ cancionx.album }})</p>
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
