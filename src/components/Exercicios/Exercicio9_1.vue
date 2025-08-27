<!-- Props -->

<script setup>
const props = defineProps({
        title: String,
        price: String,
        image: String,
        disponivel: Boolean,
    })
</script>

<template>
     <div class="cardBianca">
        <p v-if="title">{{ title }} </p>
        <span v-if="price">{{ price }} </span>
        <div id="image"><img :src="image"></div>
        <div :class="disponivel ? 'disponivel' : 'indisponivel'">{{ disponivel ? 'Disponivel' : 'Indisponivel' }}</div>
     </div>
</template>

<style scoped>
    .cardBianca{
        border: 3px solid #cd53d1;
        background-color: #581059;
        padding: 1rem;
        margin: 1rem;
    }
    .disponivel{
        color: rgb(227, 19, 223)
    }
    .indisponivel{
        color: rgb(250, 69, 69)
    }
</style>