 <template>
  <table border="1">
    <thead>
      <tr>
        <th v-for="col in columnas" :key="col">{{ col }}</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="(fila, index) in datos" :key="index">
        <td v-for="valor in fila" :key="valor">{{ valor }}</td>
      </tr>
    </tbody>
  </table>
</template>

<script>
export default {
  name: "Tabla",
  props: {
    columnas: Array,
    datos: Array
  }
}
</script>

<style scoped>
table{
margin: 0 auto; /* centra horizontalmente */
padding: 10px;
background-color:#F5B0DC;
}

th, td{
width: 250px;
padding: 5px;
border: 2px solid #D93F9F;
}
</style>