
<template>
  <div class="card">
    <img :src="itemData?.imgSrc" />
    <span :class="itemData.recommend ? 'main-description' : 'description'">
      {{ itemData?.description }}
    </span>
    <span :class="itemData.recommend ? 'main-author' : 'author'">
      作者: {{ itemData?.author }} &nbsp; 发布时间: {{ itemData?.time }}
    </span>
  </div>
</template>

<script lang="ts">
export default {
  props: ["data"],
  data() {
    console.log(this.data);
    return {
      itemData: this?.data,
    };
  },
  methods: {},
};
</script>

<style lang="less" scoped>
@import "./index.less";
</style>
