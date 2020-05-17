<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>{{ text }}</h2>
    <div style="background: red">
  <MiComponente></MiComponente> <!-- Si queremos usar un componente dentro de otro --></div>
  </div>
</template>

<script>
import MiComponente from './MiComponente.vue' // Si queremos usar un componente dentro de otro
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  components: { // Si queremos usar un componente dentro de otro
    MiComponente
  },
  data(){
    return{
      text: 'Hola Mundo desde componente!!!'
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
