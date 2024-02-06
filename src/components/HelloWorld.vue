<template>
  <div>
    <router-view></router-view>
  </div>
</template>

<script setup>
import { useRouter } from 'vue-router'

const router = useRouter()

const steps = [
  {
    path: '/step1',
    component: () => import('./Step1.vue')
  },
  {
    path: '/step2',
    component: () => import('./Step2.vue')
  },
  {
    path: '/step3',
    component: () => import('./Step3.vue')
  }
]

// Function to move to the next step
const nextStep = () => {
  const currentPath = router.currentRoute.value.path
  const currentIndex = steps.findIndex(step => step.path === currentPath)
  if (currentIndex !== -1 && currentIndex < steps.length - 1) {
    router.push(steps[currentIndex + 1].path)
  } else {
    console.log('End of tutorial')
    // You can handle what happens when the tutorial ends
  }
}
</script>

<style scoped>
/* Add your scoped styles here */
</style>
