<script setup>
import { ref } from 'vue'

let peso = ref(0)
let altura = ref(0)
let imc = ref('')

function calcularIMC() {
    imc.value = (peso.value / ((altura.value / 100) ** 2)).toFixed(2)
}
</script>

<template>
  <p>Digite seu peso:</p>
  <input type="number" v-model.peso="peso">

  <p>Digite sua altura:</p>
  <input type="number" v-model.altura="altura">

  <button @click="calcularIMC">Calcular IMC</button>

  <p v-if="imc !== null">Seu IMC é igual a {{ imc }}</p>
  <!-- Só aparece se o imc não for nula. -->
  <p v-if="imc <= 18.5">Abaixo do peso</p>
  <p v-else-if="imc <= 25">Normal</p>
  <p v-else-if="imc <= 30">Sobrepeso</p>
  <p v-else>Obesidade</p>
</template>
