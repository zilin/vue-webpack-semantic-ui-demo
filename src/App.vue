<template>
  <div id="app">
    <h3 class="ui center aligned header">{{ title }}</h3>
    <img src="./assets/logo.png">
    <hello></hello>
  </div>
</template>

<script>
import 'semantic-ui-css/semantic.min.js'
import Hello from './components/Hello'

export default {
  name: 'app',
  components: {
    Hello
  },
  data () {
    return {
      title: 'Welcome to Your Vue.js + Semantic-UI App'
    }
  }
}
</script>

<style src="semantic-ui-css/semantic.min.css"></style>
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
