<script setup>
import AppButtonLayout from './components/AppButtonLayout.vue'
import AppFlexLayout from './components/AppFlexLayout.vue'
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
    <section>
      <header>
        <h2>App Button Layout Parent Component</h2>
      </header>
      <AppButtonLayout :buttons />
    </section>
    <section>
      <header>
        <h2>App Flex Layout</h2>
      </header>
      <AppFlexLayout>
        <p v-for="{text} in buttons" :key="text">{{ text }}</p>
      </AppFlexLayout>
    </section>
  </main>
</template>

<style scoped>
header {
  margin-bottom: 4rem;
}
</style>
