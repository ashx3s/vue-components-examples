<script setup>
import AppButton from './AppButton.vue';
defineProps({
  buttons: Array
})
</script>
<template>
  <div>
    <AppButton v-for="{text, href} in buttons" :key="text" :href :text />
  </div>
</template>

<style>
div {
  display: flex;
  gap: 2rem;
}

</style>
