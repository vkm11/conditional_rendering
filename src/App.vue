<template>
  <h2 v-if="num === 0">The number is zero</h2>
  <h2 v-else-if="num < 0">The number is negative</h2>
  <h2 v-else-if="num > 0">The number is positive</h2>
  <h2 v-else>Not a number</h2>

  <!-- <div v-if="display">
  <h4>Vijaykumar</h4>
  <h4>Prajwal</h4>
  <h4>Nithin</h4>
  </div> -->

  <!-- OR -->

  <template v-if="display">
    <h4>Vijaykumar</h4>
    <h4>Prajwal</h4>
    <h4>Nithin</h4>
  </template>

<h4 v-show="showElement">Using v-show</h4>
<h4 v-if="showElement">Using v-if</h4>

</template>

<script>
export default {
  name: "App",
  data() {
    return {
      // num:'v'  // output:- not a number
      // num:1  // output:- The number is positive
      num: -1, //output:- The number is negative
      display: true,
      showElement: true,
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
