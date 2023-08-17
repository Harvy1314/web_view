<template>
  <div
    class="bg-[url('assets/bg.jpeg')] bg-cover bg-center h-screen text-white p-5 flex overflow-hidden"
  >
    <!-- 左边屏幕 -->
    <div class="flex-1 mr-5 bg-opacity-50 bg-slate-800 p-3 flex flex-col">
      <!-- 横向柱状图、雷达图、数据传递关系图 -->
      <Horizontalbar class="h-1/3 box-border pb-4" />
      <RadarBar class="h-1/3 box-border pb-4" />
      <Relation class="h-1/3" />
    </div>
    <!-- 中间屏幕 -->
    <div class="w-1/2 mr-5 flex flex-col">
      <!-- 数据总览、地图可视化 -->
      <TotalDate class="bg-opacity-50 bg-slate-800 p-3" />
      <MapChart class="bg-opacity-50 bg-slate-800 p-3 mt-4 flex-1" />
    </div>
    <!-- 右边屏幕 -->
    <div class="flex-1 bg-opacity-50 bg-slate-800 p-3 flex flex-col">
      <!-- 竖向柱状图、环形图、文档云图 -->
      <verticalBar class="h-1/3 box-border pb-4" />
      <RingBar class="h-1/3 box-border pb-4" />
      <WordCloud class="h-1/3" />
    </div>
  </div>
</template>
<script setup>
import Horizontalbar from "./components/Horizontalbar.vue";
import MapChart from "./components/MapChart.vue";
import RadarBar from "./components/RadarBar.vue";
import Relation from "./components/Relation.vue";
import RingBar from "./components/RingBar.vue";
import TotalDate from "./components/TotalDate.vue";
import verticalBar from "./components/verticalBar.vue";
import WordCloud from "./components/WordCloud.vue";
</script>
