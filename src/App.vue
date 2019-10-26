<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "app",
  components: {
    HelloWorld
  }
};
</script>

<style>
@import "~normalize.css/normalize.css";
@import "~flexboxgrid";
@import "~sanitize.css";
body {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  margin: 0;
  padding: 0;
  font-family: Montserrat, sans-serif;
  font-size: 14px;
  line-height: 1.42857143;
  color: #333;
  font-weight: 400;
  background-color: #f4f4f4;
}

ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

a,
a:hover,
a:visited {
  text-decoration: none;
  outline: 0;
}

a:active,
a:focus,
a:hover,
a:visited {
  cursor: pointer;
  text-decoration: none;
}
</style>
