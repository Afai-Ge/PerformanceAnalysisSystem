<script>
  import { Chart } from "svelte-echarts";

  const options = {
    xAxis: {
      data: ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"],
      type: "category",
    },
    yAxis: {
      type: "value",
    },
    series: [
      {
        data: [820, 932, 901, 934, 1290, 1330, 1320],
        type: "bar",
      },
    ],
  };
</script>

<div class="app">
  <Chart {options} />
</div>

<style>
  .app {
    width: 100%;
    height: 100%;
  }
</style>
