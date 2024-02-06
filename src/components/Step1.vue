<template>
  <div>
    <h1>Step 1</h1>
    <p>This is Step 1 content. Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
    <button @click="nextStep">Next Step</button>
  </div>
</template>

<script setup>
import { nextStep } from './HelloWorld.vue'
</script>

<style scoped>
/* Add your scoped styles here */
</style>
