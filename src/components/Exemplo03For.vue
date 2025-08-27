<script setup>
let nomes = ['Geovana','Livia','Camilla']
</script>

<template> 
    <ul> 
        <li v-for="(nome,index) in nomes"> {{ index +1 }}. {{ nome }}</li>
        <!-- nome dentro da pasta nomes -->
        <!-- index +1 = enumerando a lista -->
    </ul>
</template>