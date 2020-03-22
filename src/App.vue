<template>
  <div id="app">
    <img width="25%" src="./assets/logo.png">
    <SetGame/>
  </div>
</template>

<script>
import SetGame from "./components/SetGame";

export default {
  name: "App",
  components: {
    SetGame
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
