<script setup>
import { useUserStore } from '@store/userStore'

const userStore = useUserStore()
</script>

<template>
  <div class="view lazy-view">
    <h1>{{ userStore.user_id }}</h1>
    <p>这是第一个懒加载视图（LazyOne）。</p>
  </div>
</template>

<style scoped>
.lazy-view {
  padding: 1rem;
}
</style>
