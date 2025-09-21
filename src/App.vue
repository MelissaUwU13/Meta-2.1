<template>
  <div>

    <br>

    <AppHeader titulo="Sakura" />

    <br>

    <div class="contenedor-cards">
    <Card imagen="./public/cerezos1.jpg" titulo="Cultura japonesa" texto="Ver los cerezos en flor, también conocido como 'hanami', es una tradición profundamente arraigada en Japón donde la gente se reúne para disfrutar de la belleza de las flores y celebrar la llegada de la primavera." />
    <Card imagen="./public/cerezos2.png" titulo="Tipos de flores de cerezo" texto="Aunque cada flor de cerezo recibe el nombre de 'sakura', existen variedades con diferentes características, como el color y la forma de la flor."/>
    </div>

    <br><br>
    <Tabla
      :columnas="['Característica', 'Uso en Japón', 'Curiosidades']"
      :datos="[
        ['Árbol ornamental de flores rosadas','Celebraciones de Hanami', 'Sus flores duran solo 1-2 semanas'],
        ['Existen más de 200 variedades','Decoración de calles y templos', 'Algunas especies tienen flores blancas']
      ]"
    />

    <br>

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


<style>
.contenedor-cards {
  display: flex;     
  gap: 0;              
}
</style>