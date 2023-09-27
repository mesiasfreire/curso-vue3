<script setup lang="ts">

// Formas de passar props para os componentes
// interface PostProps {
//     tituloDinamico: String,
//     tituloStatico: String
// }
// defineProps<PostProps>()

//Props com valor default 
// Props Default Values​

// export interface Props {
//   tituloDinamico?: string
//   tituloStatico?: string
// }

// const props = withDefaults(defineProps<Props>(), {
//   tituloDinamico: 'Titulo Dinamico',
//   tituloStatico: 'Titulo Static'
// })


// defineProps({
//     tituloDinamico: String,
//     tituloStatico: String
// })



</script>

<template>
   <section> <slot name="header"></slot> </section>

   <section> <slot name="content"></slot> </section>
        
    <section> <slot name="rodape"></slot> 
        Rodapé // fallback
    </section>
</template>



