<script>
import Vista from './Vista.vue'
import Editor from './Editor.vue'

export default {
  data() {
    return {
      titulo: 'Texto de Prueba',
    }
  },
  components: {
    'componente-editor': Editor,
    'componente-vista': Vista,
  }
}
</script>

<template>
  <div class="container">
    <h1>Componente Hijo Editor</h1>
    <componente-editor
      v-bind:textoAEditar="titulo"
      @actualizarTexto="titulo = $event"
    />

    <h1>Componente Hijo Vista</h1>
    <componente-vista v-bind:textoAVisualizar="titulo" />
  </div>
</template>




