<template>
  <div>{{ data }}</div>
</template>

<script setup lang='tsx'>
import { computed, ref } from 'vue';

const data = ref(1)

type A = {
  a: 0 | 1
}

const aaa: A = {
  a: 1
} 

const aa = computed<A>({
  get: () => {
    return {
      a: 1
    }
  },
  set: (val) => {
    console.log(val);
  }
})
</script>

<style scoped>
</style>
