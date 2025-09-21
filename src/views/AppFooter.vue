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
button{
justify-content: center;
padding:10px;
color: white;
background-color:#F569BF;
outline: none;
text-decoration:none;
border-color: #F569BF;
border-radius: 80px;
}

button:hover {
  background-color: #d94a9c; /* un poco más oscuro al pasar el mouse */
}

footer {
  text-align: center;
  padding: 10px;
}

</style>