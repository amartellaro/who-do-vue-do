<template>
  <div id="app">
      <Header msg="Who do? Vue do!"/>
      <ToDos />
  </div>
</template>

<script>
import Header from './components/layout/Header.vue'
import ToDos from './components/ToDos.vue'


export default {
  name: 'app',
  components: {
    Header,
    ToDos
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
body {
  margin: 0;
  padding: 0;
}

</style>
