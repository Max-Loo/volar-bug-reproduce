<template>
  <div>{{ data }}</div>
</template>

<script setup lang='tsx'>
import { ref } from 'vue';

const props = withDefaults(defineProps<{
  num: number
}>(), {
  num: 1
})
// const props = defineProps<{
//   num: number
// }>()

const data = ref(1)
</script>

<style scoped>
</style>
