<script setup>
let idade = 19
</script>

<template> 
    <p v-if="idade <= 12">Criança</p>
    <p v-else-if="idade <= 18">Adolescente</p>
    <p v-else-if="idade < 60">Adulto</p>
    <p v-else>Idoso</p>
</template>



