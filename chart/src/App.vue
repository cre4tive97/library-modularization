<template>
  <div>
    <h1>Chart.js</h1>
    <BarChart />
    <LineChart />
  </div>
</template>

<script>
/* eslint-disable */
import LineChart from "./components/LineChart.vue";
import BarChart from "./components/BarChart.vue";
export default {
  components: {
    LineChart,
    BarChart,
  },
};
</script>

<style></style>
