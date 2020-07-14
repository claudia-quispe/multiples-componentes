<template>
  <div id="lista">
      <h3> {{ titulo }} </h3>
      <ol>
        <li v-for="(cancion, i) in enlaces" v-bind:key="i"><a target="blank" v-bind:href="cancion.url">{{ cancion.texto }}</a></li>
      </ol>
  </div>
</template>

<script>

export default {
  name: 'Lista',
  props: {
    titulo: String,
    enlaces: Array
  }
}

</script>
<style>
#Lista {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  padding: 30px;
  background-color: #cbe9e9;
}
</style>