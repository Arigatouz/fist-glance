<template>
  <div>
    <h1>This is product number : {{ $route.params.id }}</h1>
    <h2><a :href="products">Products Page</a></h2>
  </div>
</template>

<script>
export default {
  name: `SpecificPage`,
  validate(data) {
    console.log(data)
    console.log(data.app.head.title)
    // this regex to make sure that the params is a Number
    return /^\d+$/.test(data.params.id)
  },
  data() {
    return {
      products: '/products',
    }
  },
}
</script>
