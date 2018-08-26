<template>
  <div id="app">
    <h1>名探偵コナン 映画タイトル ジェネレーター</h1>
    <Generator/>
  </div>
</template>

<script>
import 'normalize.css'

import Generator from './components/Generator.vue'

export default {
  name: 'app',
  components: {
    Generator
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=M+PLUS+1p:400,700&subset=japanese');

#app {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  font-family: 'M PLUS 1p', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
