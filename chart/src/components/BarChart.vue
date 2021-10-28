<template>
  <div>
    <canvas ref="barChart" id="barChart" width="400" height="400"></canvas>
  </div>
</template>

<script>
/* eslint-disable */
export default {
  props: {
    barChartData: Array,
  },
  mounted() {
    const myChart = new this.$_Chart(this.$refs.barChart, {
      type: "bar",
      data: {
        labels: ["Red", "Blue", "Yellow", "Green", "Purple", "Orange"],
        datasets: this.barChartData,
      },
      options: {
        scales: {
          y: {
            beginAtZero: true,
          },
        },
      },
    });
  },
};
</script>

<style></style>
