<template>
  <div class="page">
    <Title :title="props.title" />
    <slot />
    <Icon class="icon" />
  </div>
</template>

<script setup lang="ts">
import Title from './Title.vue'
import Icon from './Icon.vue'

const props = defineProps({
  title: String
})

</script>

<style scoped>
.page {
  height: 100%;
  position: relative;
}
.icon {
  position: absolute;
  right: 10px;
  bottom: 10px;
}

</style>
<style>
.slot {
  color: #000;
}
</style>