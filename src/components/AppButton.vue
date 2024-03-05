<script setup>
defineProps({
  href: String,
  text: String
})
</script>
<template>
  <a :href="href"><span> <slot></slot></span></a>
</template>
<style scoped>
a {
  width: 220px;
  height: 220px; 
  background-color: #fff3ff;
  display: grid;
  place-items: center;
  border-radius: 50%;
}
span {
  color: black;
  font-size: clamp(1.5rem, 2.5vw, 2rem);
  font-weight: medium;
}
</style>
