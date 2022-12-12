<template>
  <div id="app">
    <TheCalculator />
    <SimpleButtonVue />
  </div>
</template>

<script>
import TheCalculator from "./components/TheCalculator.vue";
import SimpleButtonVue from "./components/SimpleButton.vue";

export default {
  name: "Calculator",
  components: {
    TheCalculator,
    SimpleButtonVue,
  },
  data() {
    return {
      displayValue: "0",
    };
  },
  methods: {
    handleInput(input) {},
  },
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
