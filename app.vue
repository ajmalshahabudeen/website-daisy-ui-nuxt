<template>
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>


<script setup lang="ts">



import { onMounted } from 'vue'
import { themeChange } from 'theme-change'


onMounted(() => {
  themeChange(false)
})

useHead({
  title: 'Daisy UI | Nuxt',
  meta: [
    { name: 'description', content: 'Daisy UI Themes' }
  ]
})



</script>