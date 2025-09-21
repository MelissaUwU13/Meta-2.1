 <template>
  <div class="tarjeta">
    <img :src="imagen" alt="Imagen" width="200">
    <p>{{ texto }}</p>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    imagen: String,
    texto: String
  }
}
</script>

<style scoped>
.tarjeta {
  border: 1px solid #ccc;
  padding: 10px;
  margin: 10px;
  text-align: center;
}
</style>
