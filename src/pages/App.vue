<script setup lang="ts">

import { ref } from "vue"

import Post from '@/components/TrabalhandoComSlots/Post.vue'

const titulo = ref('Esse é um título dinânmico')
</script>

<template>
  <section class="bg-gray-950 font-thin text-gray-300">
    <!-- <Post :tituloDinamico="titulo" tituloStatico="Titulo estático" id="123123"/> -->
    <Post>
      <!-- <template v-slot:header>{{titulo}}</template>  -->
      <template #header>{{ titulo}}</template>
    </Post>
  </section>  
</template>


