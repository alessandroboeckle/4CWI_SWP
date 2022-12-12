<template>
  <div class="operator">
    <div class="calculator">
      <button @click="emitInput('1')">1</button>
      <button @click="emitInput('2')">2</button>
      <button @click="emitInput('3')">3</button>
      <button @click="emitInput('4')">4</button>
      <button @click="emitInput('5')">5</button>
      <button @click="emitInput('6')">6</button>
      <button @click="emitInput('7')">7</button>
      <button @click="emitInput('8')">8</button>
      <button @click="emitInput('9')">9</button>
      <button @click="emitInput('0')">0</button>
      <button @click="emitInput('+')">+</button>
      <button @click="emitInput('-')">-</button>
      <button @click="emitInput('*')">*</button>
      <button @click="emitInput('/')">/</button>
      <button @click="emitInput('=')">=</button>
      <button @click="emitInput('C')">C</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Keypad",
  methods: {
    emitInput(input) {
      this.$emit("input", input);
    },
  },
};
</script>

<style scoped>
.calculator {
  margin: 0 auto;
  width: 400px;
  font-size: 40px;
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-auto-rows: minmax(50px, auto);
}
.display {
  grid-column: 1 / 5;
  background-color: #333;
  color: white;
}
.zero {
  grid-column: 1 / 3;
}
.btn {
  background-color: #f2f2f2;
  border: 1px solid #999;
}
.operator {
  background-color: orange;
  color: white;
}
</style>
