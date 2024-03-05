<script setup>
import AppButtonLayout from './components/AppButtonLayout.vue'

const buttons = [
  {
    href: "https://rcarecords.com",
    text: "More about RCA"
  },
  {
    href: "https://vuejs.org",
    text: "See RCA Artists"
  },
  { 
    href: "https://vuejs.org",
    text: "Shop Merch"
  }
]
</script>

<template>
 <main>
  <header>
    <h1>Vue Components</h1>
  </header>
<!-- Generate 3 Buttons that rotate -->
  <AppButtonLayout :buttons />
 </main> 
</template>
<style>

</style>


