<script setup>
    import {ref} from 'vue'
    let nome = ref('')
    let email = ref('')
    let idade = ref('')
    let bio = ref('')
</script>

<template> 
    <p> Nome: {{ nome }}</p>
    <input type="nome" v-model="nome">

    <p> Email: {{ email }}</p>
    <input type="email" v-model="email">

    <p> Idade: {{ idade }}</p>
    <input type="idade" v-model="idade">

    <p> Bio: {{ bio }}</p>
    <input type="Bio" v-model="bio">
</template>