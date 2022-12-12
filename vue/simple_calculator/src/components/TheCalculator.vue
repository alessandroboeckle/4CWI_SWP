<template>
  <div class="display">{{ value }}</div>
</template>

<script>
export default {
  name: "Display",
  props: {
    value: {
      type: String,
      default: "0",
    },
  },
};
</script>
