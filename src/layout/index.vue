<template>
  <div class="layout">
    <Header>Data center visualization system</Header>
    <div class="layout-content">
      <div class="layout-content-left">
        <Panel>
          <div>28° West 27/07/2024 12:00 Normal</div>
          <div>28° West 27/07/2024 12:00 Normal</div>
          <div>28° West 27/07/2024 12:00 Normal</div>
        </Panel>
        <Panel>
          <PieChart></PieChart>
        </Panel>
      </div>
      <div class="layout-content-right">
        <Panel>
          <LineCharts></LineCharts>
        </Panel>
      </div>
      <Sence></Sence>
    </div>
  </div>
</template>

<script setup lang="ts" name="Layout">
import Header from './Header.vue';
import Sence from '@/components/Sence.vue';
import Panel from '@/components/Panel/index.vue';
import LineCharts from '@/components/Charts/LineChart.vue';
import PieChart from '@/components/Charts/PieChart.vue';
</script>

<style scope>
.layout {
  width: 100vw;
  height: 100vh;
}
.layout-content {
  width: 100vw;
  height: 100vh;
  background-color: #fff;
}
.layout-content-left {
  position: absolute;
  left: 0.3rem;
  top: 70px;
  width: 30vw;
}
.layout-content-right {
  position: absolute;
  right: 0.6rem;
  top: 70px;
  width: 30vw;
}
.panel {
  margin-bottom: 0.3rem;
}
</style>
