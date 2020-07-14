<template>
  <div id="Lista">
    <img alt="Vue logo" src="./assets/logo.png">
    <Lista titulo="Blood Orange" v-bind:enlaces="BloodOrange" />
    <Lista titulo="Cuco" v-bind:enlaces="Cuco" /> 
  </div>
</template>

<script>
import Lista from './components/Lista.vue'

export default {
  name: 'App',
  components: {
    Lista
  },
  data:() => {
    return {
      //aca estan mis datos
      BloodOrange: [ //aca va mi dato interno
        {texto: 'Coastal Grooves',url: 'https://www.youtube.com/watch?v=uXLEIlQJX6A'},
        {texto: 'Cupid Deluxe', url:'https://www.youtube.com/watch?v=RBHwO-2Amzs&list=PLMNMmvIC2uGaQVq0rLqHWrSVtxdyO9fYT'},
        {texto: 'Freetown Sound', url:'https://www.youtube.com/watch?v=EK6R6WfKo0M&list=PLxKHVMqMZqUS7chrq-OLeE4rX9hYyml5B'},
        {texto: 'Negro Swan', url:'https://www.youtube.com/watch?v=3fSgsvJC9Nw&list=PLISgjPzhNbvZQXXY7qH1aG8YDf0MA27z2'},
        {texto: 'Angel`s Pulse', url:'https://www.youtube.com/watch?v=lBFdqb3P1lA&list=PLg1UyK6Rptxsan7iGWqld2Ki8Wik_PHz9'},
      ],
      Cuco: [
        {texto: 'Para Mi',url: 'https://www.youtube.com/watch?v=2qrX7n5O9m0&list=PLFJ4rD4UhAdpE1YGPME_9caqb2en6BYis'},
        {texto: 'Songs4u',url: 'https://www.youtube.com/watch?v=n-4gqm6Ah-A&list=PLmd3unaE1YCLFcQnZ6d_JJprXWChaQ0A3'},
        {texto: 'Wannabewithu',url: 'https://www.youtube.com/watch?v=9wiEM0s4aCQ&list=PLmd3unaE1YCJCplCwB04ji7SmjAgPI4QZ'},
        {texto: 'A24',url: 'https://www.youtube.com/watch?v=4iB8VUSMfjE'},
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
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
