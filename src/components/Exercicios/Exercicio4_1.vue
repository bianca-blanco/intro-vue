<script setup>
let text = '<strong>Texto</strong>'
</script>

<template>
  <div v-html="text"></div>
  <div>  {{ text }}</div>

</template>
