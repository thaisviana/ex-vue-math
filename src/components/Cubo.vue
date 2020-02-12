<template>
 <div class="card" style="width: 18rem;">
      <div class="card-body">
        <h5 class="card-title">Cubo</h5>
        <h6 class="card-subtitle mb-2 text-muted">{{ numero }}</h6>
        <p class="card-text">{{ calcula_cubo(numero) }}</p>
      </div>
    </div>
</template>

<script>
export default {
  name: 'Cubo',
  props: {
    numero: Number
  },
  methods : {
      calcula_cubo(n){
        return n ** 3 
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
