<template>
    <h1>My Num: {{ msg }}</h1>
</template>

<script setup>
import {watch} from 'vue'

const props = defineProps({
  msg: {
    type: Number,
    required: true
  }
})
watch(props, (newX) => {
  console.log(`x is ${newX.msg}`)
})
</script>