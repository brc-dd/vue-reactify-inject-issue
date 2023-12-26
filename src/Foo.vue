<script setup>
import { reactify } from '@vueuse/core'
import { inject } from 'vue'

const getA = reactify(() => inject('a').value)
</script>

<template>
  {{ getA() }}
</template>
