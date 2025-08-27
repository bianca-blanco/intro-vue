<script setup>
import { ref } from 'vue'

const estadobotao = ref('ativo')

function alternaBotao() {
  if (estadobotao.value === 'ativo') {
    estadobotao.value = 'carregando'
    setTimeout(() => {
      estadobotao.value = 'inativo'
    }, 2000)
  } else if (estadobotao.value === 'inativo') {
    estadobotao.value = 'ativo'
  }
}
</script>

<template>
  <button
    :class="estadobotao"
    :disabled="estadobotao === 'carregando'"
    @click="alternaBotao"
  >
    {{ estadobotao === 'ativo' ? 'Ativo' : estadobotao === 'carregando' ? 'Carregando...' : 'Inativo' }}
  </button>
</template>

<style scoped>
.ativo {
  color: white;
  background: rgb(180, 43, 226);
  border: 2px solid rgb(180, 43, 226);
}
.carregando {
  color: white;
  background: rgb(220, 20, 160);
  border: 2px dashed rgb(220, 20, 160);
}
.inativo {
  color: white;
  background: crimson;
  border: 2px solid crimson;
  opacity: 0.7;
}
</style>