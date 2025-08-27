<script setup>
import { ref } from 'vue'

let inputValue = ref('')

function mensagem() {
  alert(`Informação: ${inputValue.value}`)
}
</script>

<template>
  <input type="text" @keyup.down="mensagem" v-model="inputValue">

  <p>
    <input type="text" @keyup.press.9="mensagem" v-model="inputValue">
  </p>
</template>
