<template>
<div class="calculator-wrapper">
  <div class="calculator-screen">
    <div class="screen-print">7812</div>
  </div>
  <div class="calculator-body">
    <div class="first-row">
      <div class="calculator-button">C</div>
      <div class="calculator-button">+/-</div>
      <div class="calculator-button">%</div>
      <div class="calculator-button button-yellow">/</div>
    </div>
    <div class="second-row">
      <div class="calculator-button">7</div>
      <div class="calculator-button">8</div>
      <div class="calculator-button">9</div>
      <div class="calculator-button button-yellow">X</div>
    </div>
    <div class="third-row">
      <div class="calculator-button">4</div>
      <div class="calculator-button">5</div>
      <div class="calculator-button">6</div>
      <div class="calculator-button button-yellow">-</div>
    </div>
    <div class="fourth-row">
      <div class="calculator-button">1</div>
      <div class="calculator-button">2</div>
      <div class="calculator-button">3</div>
      <div class="calculator-button button-yellow">+</div>
    </div>
    <div class="fifth-row">
      <div class="calculator-button">0</div>
      <div class="calculator-button">.</div>
      <div class="calculator-button"></div>
      <div class="calculator-button button-yellow">=</div>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'Calculator',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.calculator-wrapper {
  width: 400px;
  margin: 2em auto;
  background: red;
  display: flex;
  flex-direction: column;
}

.calculator-screen {
  height: 100px;
  background: lightslategray;
  border: .5px solid grey;
  display: flex;
  justify-content: flex-end;
}

.screen-print {
  color: white;
  text-align: right;
  align-self: center;
  margin-right: 20px;
  font-size: 25px;
  letter-spacing: 3px;
}

.calculator-body {
  display: flex;
  flex-direction: column;
}

.first-row,
.second-row,
.third-row,
.fourth-row,
.fifth-row {
  display:flex;
}

.calculator-button {
  width: 25%;
  text-align: center;
  padding: 20px;
  background: lightgrey;
  border: .5px solid grey;
}


.button-yellow {
  background: #f5c542;
  color: white;
}

</style>
