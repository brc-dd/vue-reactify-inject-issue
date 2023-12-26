<script setup>
import { provide, ref } from 'vue'
import Foo from './Foo.vue'

const a = ref(2)

provide('a', a)
</script>

<template>
  <Foo />
  <br />
  <button @click="a++">a++</button>
</template>
