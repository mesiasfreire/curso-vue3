<!-- <template>
    <div class="w-4/5" >
        <component :is='currentComponent'></component>
    </div>
</template>

<script setup lang="ts">

import {ref, computed, defineAsyncComponent} from 'vue'
const AlertInfo = defineAsyncComponent(() =>
  import('./AlertInfo.vue')
)
const AlertError = defineAsyncComponent(() =>
  import('./AlertError.vue')
)

const borderColor = ref('')

const currentComponent = computed(() => );


</script>

<style scoped>

</style> -->