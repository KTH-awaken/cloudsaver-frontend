<template>
  <div>
    <h1>Step 2</h1>
    <p>This is Step 2 content. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
    <button @click="nextStep">Next Step</button>
  </div>
</template>

<script setup>
import { nextStep } from './HelloWorld.vue'
</script>

<style scoped>
/* Add your scoped styles here */
</style>
