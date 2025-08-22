<template>
  <!-- Acá va el HTML -->

  <p>{{ contador }}</p>
  <button @click = "Incrementar">Incrementar</button>
  <button @click = "Decrementar">Decrementar</button>
</template>

<script setup>
  /*Acá va la lógica en JavaScript*/ 

  import {ref} from 'vue'
  const contador = ref(0)

  const Incrementar = () =>{
    contador.value++
  }
  const Decrementar = () =>{
    contador.value--
  }
</script>

<style scoped>
  /*Acá va el CSS*/

  p{
    color: deeppink;
  }
</style>
