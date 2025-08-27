<script setup>
let usuariologado = false

</script>

<template> 
    <p v-if="usuariologado == false">Faça login </p>
    <p v-else="usuariologado == true">Bem-Vindo</p>

</template>


