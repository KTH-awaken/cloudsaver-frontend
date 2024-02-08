<template>
  <div>
    <h1>Step 3</h1>
    <p>This is Step 3 content. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.</p>
    <button @click="nextStep">Next Step</button>
  </div>
</template>

<script setup>
import { nextStep } from './HelloWorld.vue'
</script>

<style scoped>
/* Add your scoped styles here */
</style>
