<template>
  <footer>
      <a :href="link" target="_blank">
      <button>Da click para más información</button>
    </a>
  </footer>
</template>

<script>
export default {
  name: "AppFooter",
  props: {
    link: String // ruta o URL que se recibe como prop
  }
}
</script>

<style scoped>
a{
justify-content: center;
padding:10px;
color: white;
background-color:#F569BF;
outline: none;
text-decoration:none;
border-radius: 80px;
}
</style>