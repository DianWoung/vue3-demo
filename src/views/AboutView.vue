<template>
  <div class="about">
    <h1>This is an about page</h1>
    <button @click="parentMsg++">数字追加器</button>
    <Son :msg="parentMsg" />
  </div>
</template>

<script setup>
import { ref } from 'vue'
import Son from '../components/Son.vue'
const parentMsg = ref(1)
</script>


<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
