<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <div>修改A</div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import _ from 'lodash';

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data() {
    return {
      arr: [1,2,3,4,5],
    }
  },
  mounted() {
    console.log(_.fill(this.arr, 'a'))
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
