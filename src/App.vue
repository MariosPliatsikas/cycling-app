<!-- src/App.vue -->

<template>
  <div id="app">
    <CyclingData />
  </div>
</template>

<script>
import CyclingData from './components/CyclingData.vue';

export default {
  components: {
    CyclingData,
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
