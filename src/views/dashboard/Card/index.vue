<template>
  <div>
    <el-row :gutter="10">
      <el-col :span="6">
        <el-card>
          <Detail title="总销售额" count="88406">
            <template slot="charts">
              <span
                >周同比&nbsp;&nbsp;56.67%
                <svg
                  t="1651913345219"
                  class="icon"
                  viewBox="0 0 1024 1024"
                  version="1.1"
                  xmlns="http://www.w3.org/2000/svg"
                  p-id="5806"
                  width="16"
                  height="16"
                  data-spm-anchor-id="a313x.7781069.0.i13"
                >
                  <path
                    d="M512 618.666667L298.666667 405.333333h426.666666L512 618.666667z"
                    fill="#d81e06"
                    p-id="5807"
                    data-spm-anchor-id="a313x.7781069.0.i14"
                    class="selected"
                  ></path>
                </svg>
              </span>
              <span>
                日同比&nbsp;&nbsp;19.96%
                <svg
                  t="1651914480484"
                  class="icon"
                  viewBox="0 0 1024 1024"
                  version="1.1"
                  xmlns="http://www.w3.org/2000/svg"
                  p-id="6556"
                  width="16"
                  height="16"
                >
                  <path
                    d="M512 405.333333L298.666667 618.666667h426.666666L512 405.333333z"
                    fill="#1afa29"
                    p-id="6557"
                  ></path>
                </svg>
              </span>
            </template>
            <template slot="footer">
              <span>日销售额￥ 12423</span>
            </template>
          </Detail>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card>
          <Detail title="访问量" count="88406">
            <template slot="charts">
                <lineChart></lineChart>
            </template>
            <template slot="footer">
              <span>日访问量 1234</span>
            </template>
          </Detail>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card>
          <Detail title="支付笔数" count="88406">
            <template slot="charts">
                <barChart></barChart>
            </template>
            <template slot="footer">
              <span>转换率64%</span>
            </template>
          </Detail>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card>
          <Detail title="运营活动效果" count="88406">
            <template slot="charts"> 
                <progressChart></progressChart>
            </template>
            <template slot="footer">
              <span
                >周同比&nbsp;&nbsp;56.67%
                <svg
                  t="1651913345219"
                  class="icon"
                  viewBox="0 0 1024 1024"
                  version="1.1"
                  xmlns="http://www.w3.org/2000/svg"
                  p-id="5806"
                  width="16"
                  height="16"
                  data-spm-anchor-id="a313x.7781069.0.i13"
                >
                  <path
                    d="M512 618.666667L298.666667 405.333333h426.666666L512 618.666667z"
                    fill="#d81e06"
                    p-id="5807"
                    data-spm-anchor-id="a313x.7781069.0.i14"
                    class="selected"
                  ></path>
                </svg>
              </span>
              <span>
                日同比&nbsp;&nbsp;19.96%
                <svg
                  t="1651914480484"
                  class="icon"
                  viewBox="0 0 1024 1024"
                  version="1.1"
                  xmlns="http://www.w3.org/2000/svg"
                  p-id="6556"
                  width="16"
                  height="16"
                >
                  <path
                    d="M512 405.333333L298.666667 618.666667h426.666666L512 405.333333z"
                    fill="#1afa29"
                    p-id="6557"
                  ></path>
                </svg>
              </span>
            </template>
          </Detail>
        </el-card>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import Detail from "./Detail";
import lineChart from "./lineChart";
import barChart from "./barChart";
import progressChart from "./progressChart";

export default {
  name: "Card",
  components: {
    Detail,
    lineChart,
    barChart,
    progressChart,
  },
};
</script>

<style>
</style>