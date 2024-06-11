<template>
  <div id="app">
    <PDF />
  </div>
</template>

<script>
import PDF from './pages/PDF.vue'

export default {
  name: 'App',
  components: {
    PDF
  }
}
</script>

<style scoped>
#app {
  font-family: 'Averta';
  width: 210mm;
}
</style>