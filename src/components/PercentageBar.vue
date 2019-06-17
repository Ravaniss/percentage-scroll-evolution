<template>
  <div class="percentage-bar" :style="emptyBar">
    <div class="fill" :style="progressBar"></div>
  </div>
</template>

<script lang="ts">

import { Component, Vue, Prop } from 'vue-property-decorator'

@Component
export default class PercentageBar extends Vue {
  @Prop() emptyBar: any;
  @Prop() progressBar: any;
}
</script>


<style lang="scss" scoped>
  div.percentage-bar {
    position: relative;
    width: 100%;
    max-width: 530px;
    height: 12px;
    margin: 0 auto;
    background-color: #171717;

    .fill {
      position: absolute;
      width: 0;
      top: 0;
      left: 0;
      bottom: 0;
      background-color: #FFCE00;
      z-index: 0;
    }
  }
</style>

