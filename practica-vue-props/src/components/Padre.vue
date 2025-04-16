<script>
import Vista from './components/Vista.vue'
import Editor from './components/Editor.vue'


export default{
  data(){
    return{
      titulo: '',
    }
  },
  components: {
    'componente-editor': Editor,
    'componente-vista': Vista,
  },
}


</script>


<template>
  <h1>Componente Hijo Editor</h1>
  <componente-editor v-bind:textoAEditar=""/>

  <h1>Componente Hijo Vista</h1>
  <componente-vista/>
</template>



