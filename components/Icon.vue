<template>
  <img :src="props.path" class="icon" />
</template>

<script setup lang="ts">
const props = defineProps({
  path: {
    type: String,
    default: 'icon.png'
  }
})
</script>

<style>
.icon {
  width: 50px;
  height: 50px;
  border-radius: 50px;
  border: 1px solid palevioletred;
  padding: 1px;
}
</style>