<template>
  <div id="app">
    <h1>名探偵コナン 映画タイトル ジェネレーター</h1>
    <Generator/>
  </div>
</template>

<script>
import 'normalize.css'
import 'bulma/css/bulma.css'

import Generator from './components/Generator.vue'

export default {
  name: 'app',
  components: {
    Generator
  },
  mounted: function() {
    this.loadFont();
  },
  methods: {
    loadFont: function() {
      document.addEventListener("DOMContentLoaded", function() {
        var link = document.createElement("link");
        link.type = "text/css";
        link.rel = "stylesheet";
        link.href =
          "https://fonts.googleapis.com/css?family=M+PLUS+1p:400,700&subset=japanese";
        document.head.appendChild(link);
      });
    }
  }
}
</script>

<style>
#app {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  font-family: 'Noto Sans JP', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
h1 {
  margin-bottom: 1rem;
}
</style>
