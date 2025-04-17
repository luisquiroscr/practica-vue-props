<script>

export default{
  props: {
    textoAEditar: {
      type: String,
      required: true
    }
  }
}

</script>

<template>
  <div class="container">
    <h1>Editor de texto</h1>
    <input
      :value="textoAEditar"
      @input="$emit('actualizarTexto', $event.target.value)"
    />
  </div>
</template>
