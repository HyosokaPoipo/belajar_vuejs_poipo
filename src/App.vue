<template>
  <div id="app">
    <img src="./assets/logo.png">
    <h1>{{ title }}</h1>
    <a :href="hisoka_website"> my blog </a>
    <input type="text" :value="hisoka_name"> </input>
    <p v-html="hisoka_html"></p>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      title: 'Contoh v-bind',
      hisoka_website: 'http://dimensitutupbotol.blogspot.co.id',
      hisoka_name: 'Hisoka Poipo',
      hisoka_html:'<a href="http://dimensitutupbotol.blogspot.co.id"> hisoka blog </a>'
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
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
