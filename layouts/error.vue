<template>
  <div>
    <div class="main-div">
      <h1 v-if="error.statusCode === 404">Page not found</h1>
      <h1 v-else>An error occurred</h1>
    </div>
    <div class="home-page-link">
      <NuxtLink to="/">Home page</NuxtLink>
    </div>
  </div>
</template>

<script>
export default {
  props: ['error'],
}
</script>

<style scoped>
.main-div {
  display: flex;
  align-items: center;
  justify-content: center;
}
.home-page-link {
  font-size: 20px;
  font-weight: bold;
}
</style>
