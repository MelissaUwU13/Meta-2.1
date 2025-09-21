<template>
  <header>
    <h1>{{ titulo }}</h1>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  props: {
    titulo: String
  }
}
</script>

<style scoped>
h1{
display: flex;
justify-content: center;
background-image: url("./public/banner.jpg");
color:black;
}
</style>