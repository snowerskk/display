<template>
  <h1 class="title">{{ props.title }}</h1>
</template>

<script setup lang="ts">
const props = defineProps({
  title: String
})
</script>

<style scoped>
.title {
  margin-bottom: 1rem;
  margin-left: -0.05em;
  font-size: 2.25rem;
  line-height: 2.5rem;
  text-align: center;
  color: #2F4F4F;
}
</style>
