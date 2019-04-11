<template>
  <div id="app">
      <Header msg="Who do? Vue do!"/>
      <ToDoInput msg="What would you like to do?"/>
  </div>
</template>

<script>
import Header from './components/layout/Header.vue'
import ToDoInput from './components/ToDoInput.vue'

export default {
  name: 'app',
  components: {
    Header,
    ToDoInput
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
