<template>
  <div>
    <header></header>
    <nuxt />
    <footer></footer>
  </div>
</template>

<script>
export default {}
</script>

<style>
*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

header,
footer {
  height: 80px;
  width: 100%;
  background-color: #333;
  color: #fff;
  text-align: center;
  font-size: 20px;
  padding-top: 25px;
}
footer {
  position: fixed;
  bottom: 0;
}
</style>
