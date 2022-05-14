<template>
  <div>
    <h1>Hello From the product page</h1>
    <input
      type="text"
      placeholder="Enter the product Number"
      v-model="productNumber"
    />
    <button @click="loadProduct">GO to the product</button>
    <div>
      <h3><nuxt-link to="/products/1">product One</nuxt-link></h3>
      <h3><nuxt-link to="/products/2">product Two</nuxt-link></h3>
    </div>
    <a href="/">Go back</a>
  </div>
</template>
<script>
export default {
  name: 'products',
  data() {
    return {
      productNumber: '',
    }
  },
  methods: {
    loadProduct() {
      this.$router.push(`/products/${this.productNumber}`)
    },
  },
}
</script>
