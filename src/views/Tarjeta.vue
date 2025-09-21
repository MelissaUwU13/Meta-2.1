 <template>
  <div class="tarjeta">
    <img :src="imagen" alt="Imagen" class="card-img">
    <br>
    <h5>{{ titulo }}</h5>
    <br>
    <p>{{ texto }}</p>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    imagen: String,
    titulo: String,
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

.card-img {
  width: 100%;
  height: auto;
  display: block;
}
</style>
