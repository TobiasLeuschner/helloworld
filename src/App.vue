<template>
  <div id="app">
  Hallo {{fullName}} ich bin {{ new Date().getFullYear() - byear}} Jahre alt
  </div>
</template>

<script>

export default {
  name: 'App',
  data: () =>({
    lastname: 'Schüppi',
    vorname: 'David',
    byear: 1996
  }),
  computed: {
    fullName(){
      return this.vorname + " " + this.lastname;
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
</style>
