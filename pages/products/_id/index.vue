<template>
  <div>
    <h1>This is product number : {{ $route.params.id }}</h1>
    <h2><a :href="products">Products Page</a></h2>
  </div>
</template>

<script>
export default {
  data() {
    return {
      products: '/products',
    }
  },
}
</script>
