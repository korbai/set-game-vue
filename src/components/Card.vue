<template>
  <div class="card" :style="{ backgroundColor :color }">
    <h1>CARD</h1>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    color: {
      type: String,
      required: true
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
