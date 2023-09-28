<script setup lang="ts">


// defineProps(['titulo','subtitulo'])
const emit = defineEmits(['clicou'])


const props = defineProps({
    titulo: { type: String, required: true },
    subtitulo: { type: String }
})

const handleEventEmitter = (()=> emit("clicou", 3))

</script>
<template>
    <div>
        <h1>{{ titulo }}</h1>
        <h2>{{ subtitulo }}</h2> 
        <slot></slot>
        <button @click="handleEventEmitter"> Emitir Evento</button>
    </div>
</template>


