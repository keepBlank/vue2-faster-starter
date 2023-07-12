<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <g-button>UI组件库</g-button>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import { GButton,GButtonGroup,GIcon } from 'g-design-of-vue';
import '../node_modules/g-design-of-vue/dist/index.css'

export default {
  name: 'App',
  components: {
    'g-button': GButton,
    HelloWorld
  }
}
</script>

<style>
  html {
  --button-height: 32px;
  --font-size: 14px;
  --button-bg: white;
  --button-active-bg: #eee;
  --border-radius: 4px;
  --color: #333;
  --border-color: #999;
  --border-color-hover: #666;
  --border-active-bg: #d3d2d2;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
