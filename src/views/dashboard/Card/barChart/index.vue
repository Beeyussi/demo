<template>
  <div class="chart" ref="chart"></div>
</template>

<script>
import echarts from "echarts";
export default {
  name: "barChart",
  mounted() {
    let barCharts = echarts.init(this.$refs.chart);
    barCharts.setOption({
      xAxis: {
        show: false,
        type: "category",
      },
      yAxis: {
        show: false,
      },
      series: [
        {
          type: "bar",
          data: [10, 76, 39, 48, 33, 94],
          color:'pink'
         
        },
      ],
      grid: {
        left: 0,
        top: 0,
        right: 0,
        bottom: 0,
      },
       tooltip:{},
    });
  },
};
</script>

<style>
.chart {
  width: 100%;
  height: 100%;
}
</style>