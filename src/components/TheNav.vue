<script setup>
const links = [
   {
    href: "https://rcarecords.com",
    text: "About"
  },
  {
    href: "https://vuejs.org",
    text: "Gallery"
  },
  {
    href: "https://vuejs.org",
    text: "Shop"
  }
]
</script>
<template>
  <nav>
    <div>
      Logo
    </div>
    <ul>
      <li v-for="{href, text} in links "><a :href>{{ text }}</a></li>
    </ul>
  </nav>
  <div>
    <span>btn</span>
    <span>btn</span>
    <span>btn</span>
  </div>
</template>

<style scoped>

</style>