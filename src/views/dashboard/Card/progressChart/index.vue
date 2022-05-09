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
        max: 100,
        min: 0,
      },
      yAxis: {
        show: false,
        type: "category",
      },
      series: [
        {
          type: "bar",
          data: [76],
          color: "yellowgreen",
          barWidth: 10,
          showBackground: true,
          backgroundStyle: {
            color: "#eee",
          },
          label: {
            show: true,
            formatter: "|",
            //文本标签位置调试
            position: "right",
          },
        },
      ],
      grid: {
        left: 0,
        top: 0,
        right: 0,
        bottom: 0,
      },
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