<script setup>
    let validacao = false
    let isError = false
    let isActive = true
    let isDisable = false
</script>

<template>
    <!-- <p :class="validacao ?'ok' : 'falha'">Utilizando a diretiva classe</p> -->
     <p :class="{
        'ok': isActive,
        'falha': isError
     }" >Teste Diretiva Class</p>

     <button :disable="isDisable">Clique Aqui</button>

</template>

<style scoped>
.ok{
    color: blueviolet;
}

.falha{
    color: crimson;
}

</style>