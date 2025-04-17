<script>
export default {
  props: {
    textoAVisualizar: {
      type: String,
      require: true
    }
  }
}
</script>

<template>
  <p>{{ textoAVisualizar }}</p>
</template>
