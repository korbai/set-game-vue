<template>
  <div
    class="card card-type-${type}"
    :style="{ backgroundColor :color }"
    style="padding: 2px; margin: 8px; height: ${height}; width: ${width}; display: inline-block;"
  >
    <svg
      xmlns="http://www.w3.org/2000/svg"
      version="1.1"
      :width="width"
      :height="height"
      viewBox="0 0 60 90"
    >
      <defs>
        <pattern id="fillPatternRed" x="6" y="6" width="5" height="5" patternUnits="userSpaceOnUse">
          <rect x="2" y="0" width="2" height="2" fill="#ff0000"></rect>
          <rect x="1" y="1" width="2" height="2" fill="#ff0000"></rect>
          <rect x="0" y="2" width="2" height="2" fill="#ff0000"></rect>
        </pattern>
        <pattern
          id="fillPatternGreen"
          x="6"
          y="6"
          width="5"
          height="5"
          patternUnits="userSpaceOnUse"
        >
          <rect x="2" y="0" width="2" height="2" fill="#007f00"></rect>
          <rect x="1" y="1" width="2" height="2" fill="#007f00"></rect>
          <rect x="0" y="2" width="2" height="2" fill="#007f00"></rect>
        </pattern>
        <pattern
          id="fillPatternPurple"
          x="6"
          y="6"
          width="5"
          height="5"
          patternUnits="userSpaceOnUse"
        >
          <rect x="2" y="0" width="2" height="2" fill="#7f007f"></rect>
          <rect x="1" y="1" width="2" height="2" fill="#7f007f"></rect>
          <rect x="0" y="2" width="2" height="2" fill="#7f007f"></rect>
        </pattern>
      </defs>
      <g>
        <rect ry="5" rx="5" stroke="#7f7f00" height="90" width="60" y="0" x="0" fill="#ffffdd"></rect>
        ${body}
      </g>
    </svg>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    color: {
      type: String,
      required: true
    },
    width: {
      type: Number,
      required: true,
      default: 60
    },
    height: {
      type: Number,
      required: true,
      default: 90
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
