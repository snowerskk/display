<template>
  <span class="text">{{ props.text }}</span>
</template>

<script setup lang="ts">
const props = defineProps({
  text: String
})

</script>

<style scoped>
.text {
  display: inline-block;
  color: #79bbff;
  border: 1px solid #79bbff;
  color: #000;
  border: 1px solid #000;
  background: #d9ecff;
  font-size: 12px;
  border-radius: 4px;
  padding: 2px;
  margin-right: 2px;
}
</style>
