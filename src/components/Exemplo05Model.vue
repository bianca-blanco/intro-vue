<script setup>
    import {ref} from 'vue'
    let texto = ref('')
</script>
<!-- ref - reativa
- sempre que a variável mudar ela vai atualizar sozinha no prompt 
- usar ref na variávle torna ela um objeto (por isso q para acessar precisa ser nomedavariável.value -->

<template>
    <input type="text" v-model="texto">
    <p> Valor do input: {{ texto }}</p>
</template>

