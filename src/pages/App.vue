<script setup lang="ts">
import { ref, onMounted } from 'vue'
const titulo = ref('')
const el = ref<HTMLElement | null>(null)
import Componente from "@/components/PrimeiroComponente/Componente.vue"
import CustomInput from "@/components/CustomInput.vue";
import Alerta from "@/components/PrimeiroComponente/Alerta.vue"


onMounted(() => {
  console.log(el)
});
</script>

<template>
  <section class="w-screen h-screen bg-gray-200 p-2" ref="el">
    <Alerta ref="alert"> 
      <template #header>
        Titulo de erro
      </template>
      <template v-slot:conteudo>Eesse é o conteudo do erro</template>
    </Alerta>
   <Componente subtitulo="subtitulo" :titulo="titulo" @clicou="(e)=> console.log(e)">
   <CustomInput  v-model="titulo"/>
    
  </Componente>

    
    </section>  
</template>


