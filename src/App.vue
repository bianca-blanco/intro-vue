
<script setup>

// import UserCard from './components/Exemplo10Props.vue'
//   const user = {
//     nome: String,
//     email: String,
//     idade: Number,
//     telefone: String,
//     ativo: Boolean
//   }

// import Exemplo01 from './components/Exemplo01Interpolacao.vue'
// import Exemplo1_1 from './components/Exercicios/Exercício1_1.vue'
// import Exemplo1_2 from './components/Exercicios/Exercicio1_2.vue'
// import Exemplo1_3 from './components/Exercicios/Exercicio1_3.vue'
// import Exemplo02 from './components/Exemplo02Condicional.vue';
// import Exemplo2_1 from './components/Exercicios/Exercicio2_1.vue';
// import Exemplo2_2 from './components/Exercicios/Exercicio2_2.vue';
// import Exemplo03For from './components/Exemplo03For.vue';
// import Exemplo03For from './components/Exemplo03For.vue';
// import Exercicio3_1 from './components/Exercicios/Exercicio3_1.vue'
// import Exercicio3_2 from './components/Exercicios/Exercicio3_2.vue'
// import Exemplo04 from './components/Exemplo04HTML.vue'
// import Exercicio4_1 from './components/Exercicios/Exercicio4_1.vue'
// import Exemplo05 from './components/Exemplo05Model.vue'
// import Exercicio5_1 from './components/Exercicios/Exercicio5_1.vue'
// import Exercicio5_2 from './components/Exercicios/Exercicio5_2.vue'
// import Exemplo06 from './components/Exemplo06Classe.vue'
// import Exercicio6_1 from './components/Exercicios/Exercicio6_1.vue'
// import Exemplo07 from './components/Exemplo07Clique.vue'
// import Exercicio7_1 from './components/Exercicios/Exercicio7_1.vue'
// import Exemplo08 from './components/Exemplo08Teclado.vue'
// import Exercicio8_1 from './components/Exercicios/Exercicio8_1.vue'
// import Exemplo09 from './components/Exemplo09Enter.vue'
// import Exemplo10 from './components/Exemplo10Props.vue' (ta la em cima pq definiu o que vai em cada campo e colocou nome diferente)
// import Exercicio9_1 from './components/Exercicios/Exercicio9_1.vue'
// import Pesquisa from './components/Pesquisa.vue'
// import Baselayout from './Baselayout.vue';
import BaseLayout from './components/BaseLayout.vue'

// import { ref } from 'vue'
// import Exercicio10_1 from './components/Exercicios/Exercicio10_1.vue'

// const produtos = ref([
//     { nome: 'Blush: Vizzela', price: 35.97 },
//     { nome: 'Balm: Ruby Rose Feels', price: 40.00 },
//     { nome: 'Rímel: Melu', price: 19.83 }
// ])

// const mensagemCompra = ref('')

// function handleBuy(nomeProduto) {
//     const msg = `Você comprou ${nomeProduto}`
//     mensagemCompra.value = msg
//     console.log(msg)
// }

// exemplo 11 (coisas necessárias)
// import {ref} from 'vue'
// import Exemplo11 from './components/Exemplo11Emits.vue'
// const totalCliques = ref(0)

// function atualiazarTotal(valor){
//   totalCliques.value = valor
// }

</script>


<template>
  <Exemplo01> </Exemplo01>
  <Exemplo1_1> </Exemplo1_1>
  <Exemplo1_2> </Exemplo1_2>
  <Exemplo1_3> </Exemplo1_3>
  <Exemplo02> </Exemplo02>
  <Exemplo2_1> </Exemplo2_1>
  <Exemplo2_2></Exemplo2_2>
  <Exemplo03For> </Exemplo03For>
  <Exercicio3_1> </Exercicio3_1>
  <Exercicio3_2> </Exercicio3_2>
  <Exemplo04> </Exemplo04>
  <Exercicio4_1> </Exercicio4_1>
  <Exemplo05> </Exemplo05>
  <Exercicio5_1> </Exercicio5_1>
  <Exercicio5_2> </Exercicio5_2>
  <Exemplo06> </Exemplo06>
  <Exercicio6_1> </Exercicio6_1>
  <Exemplo07> </Exemplo07>
  <Exercicio7_1> </Exercicio7_1>
  <Exemplo08> </Exemplo08>
  <Exercicio8_1> </Exercicio8_1>
  <Exemplo09> </Exemplo09>
  <!-- <Exemplo10> </Exemplo10> o de baixo aí, só que definindo o q vai em cada campo (do card) -->
  <!-- <UserCard nome="Bianca" email="bianca@gmail.com" idade="17" telefone="11928739471" Inativo="False"></UserCard>
  <Exercicio9_1 title="Stuart" price="Doação" image="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQwFpQ_7rXdlBDeBE6VCYf-S7wQNBR2hU0udQ&s" :disponivel="true"></Exercicio9_1> -->
  <!-- <Exemplo11 @update="atualiazarTotal"></Exemplo11> -->
  <!-- <p>Total de cliques: {{ totalCliques }}</p> -->
<!-- 
  <h2>Produtos</h2>
    <div style="display: flex; gap: 1rem; flex-wrap: wrap;">
        <Exercicio10_1
            v-for="(produto, i) in produtos"
            :key="produto.nome + i"
            :nome="produto.nome"
            :price="produto.price"
            @buy="handleBuy"
        />
    </div>
    <p v-if="mensagemCompra" style="font-weight: bold; color: #e0aaff; margin-top: 1rem;">{{ mensagemCompra }}</p> -->
<Pesquisa> </Pesquisa>
    <PesquisaSlots>
  <!-- Exemplo do w3schools -->
  <!-- <cardSlot>
  <div>
    <h3>Slots Vue</h3>
    <p>Slots são áreas definidas em um componente filho onde o componente pai pode inserir seu próprio conteúdo.
</p>
    <slot-comp>Bianca Blanco</slot-comp>
  </div>
  </cardSlot> -->
  <!-- O conteúdo dentro de <Card> será colocado no slot -->
</PesquisaSlots>

 <BaseLayout>
    <template #header>
      <h1>Aqui nós temos um título</h1>
    </template>

    <template #default>
      <p>Um parágrafo de texto.</p>
      <p>E um conteúdo adicional.</p>
    </template>

    <template #footer>
      <p>Aqui tem informações que normalmente se tem em rodapé</p>
    </template>
  </BaseLayout>

</template>

<!-- Slots normal -->
<!-- <style>
  p {
    width: 200px;
  }
  #app div {
    border: dashed black 1px;
    margin: 10px;
    padding: 10px;
    display: inline-block;
  }
</style>

 -->
