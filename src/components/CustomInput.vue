<script setup lang="ts">
defineProps(['modelValue'])
defineEmits(['update:modelValue'])

</script>

<template>
  <input
  class="border-gray-500 focus:border-blue-300 rounded-lg"
    :value="modelValue"
    @input="$emit('update:modelValue', ($event.target as HTMLInputElement).value)"
  />
</template>