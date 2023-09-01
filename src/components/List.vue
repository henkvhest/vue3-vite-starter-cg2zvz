<template>
  <ul class="list">
    <slot></slot>
    <li>a</li>
    <li>b</li>
    <li>c</li>
  </ul>
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)
</script>

<style lang="scss" scoped>
.list > li + li {
  margin-top: 16px;
  padding: 0;
}
</style>
