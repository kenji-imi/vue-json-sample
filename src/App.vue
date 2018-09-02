<template>
  <div id="app">
    <h2>東京23区一覧</h2>
    <div v-for="(city, i) in cities" v-bind:key="i">
      {{city.id}} : {{city.name}}<br>
    </div>
  </div>
</template>

<script>
import cities from "./assets/cities.json"

export default {
  name: 'app',
  data () {
    return {
      cities
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
