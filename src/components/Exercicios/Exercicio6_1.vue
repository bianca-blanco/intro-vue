<script setup>
    let isActive = false
    let isDowload = false
    let isDisable = true
</script>

<template>

     <button :class="{
        'ok': isActive,
        'carregando': isDowload,
        'falha': isDisable
     }" :disable="isDisable">Clique Aqui</button>

</template>

<style scoped>
.ok{
    color: rgb(180, 43, 226);
}

.carregando{
    color: rgb(220, 20, 160)
}

.falha{
    color: crimson;
}

</style>