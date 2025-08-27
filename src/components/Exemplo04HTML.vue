<script setup>
let text = '<p style="color:red"> Testando a diretiva v-html'
</script>

<template>
<div v-html= "text"></div>
<!-- v-html interpreta o html inserido -->
<div> {{ text }}</div>
</template>