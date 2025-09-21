<template>
  <div>
    <AppHeader titulo="Sakura" />

    <Card imagen="./public/cerezos1.jpg" texto="Primera tarjeta" />
    <Card imagen="./public/cerezos2.png" texto="Segunda tarjeta" />

    <Tabla
      :columnas="['Característica', 'Uso en Japón', 'Curiosidades']"
      :datos="[
        ['>Árbol ornamental de flores rosadas','Celebraciones de Hanami', 'Sus flores duran solo 1-2 semanas'],
        ['Existen más de 200 variedades','Decoración de calles y templos', 'Algunas especies tienen flores blancas']
      ]"
    />
    
    <AppFooter link="https://www.viverosshangai.es/10-cosas-que-no-sabias-acerca-del-arbol-de-cerezo" />
  </div>
</template>

<script>
import AppHeader from "./views/AppHeader.vue"
import Card from "./views/Tarjeta.vue"
import Tabla from "./views/Tabla.vue"
import AppFooter from "./views/AppFooter.vue"

export default {
  name: "App",
  components: {
    AppHeader,
    Card,
    Tabla,
    AppFooter
  }
}
</script>