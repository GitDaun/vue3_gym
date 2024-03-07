<template>
  <div>
    <h2>Home View</h2>
    <p>{{ $route.path }}</p>
    <p>{{ $route.name }}</p>
    <button class="btn btn-primary" @click="movePage">about 페이지 이동</button>
  </div>
</template>

<script setup>
import { useRouter } from 'vue-router';

const router = useRouter()
const movePage = () => {
  router.push('/about')
}

</script>

<style lang="scss" scoped>

</style>