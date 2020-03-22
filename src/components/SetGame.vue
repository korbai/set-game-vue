<template>
  <div class="hello">
    <h1>Set Game</h1>
    <h3>Vue Edition</h3>
    <Card color="red"/>
  </div>
</template>

<script>
import Card from "./Card";

export default {
  name: "SetGame",
  components: {
    Card
  },
  props: {}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 20px 0 0;
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
