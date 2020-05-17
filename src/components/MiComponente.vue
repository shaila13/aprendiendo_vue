<template>
<div> <!-- Siempre hay que meterlo en un div -->
<hr/>
    <h1>{{ msg }}</h1>
    <h2>Este es mi componente</h2>
    <h3>{{ subtitulo }}</h3>
<hr/>
</div>
</template>

<script>
export default {
  name: 'MiComponente',
  props: {
    msg: String
  },
  data(){
    return{
      subtitulo: 'Soy el subtitulo de mi componente'
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
