
<template>
  <div class="header">
    <div class="item" @click="toMitrade">Mitrade官网</div>
    <div class="item" @click="toWebTrade">网页版交易</div>
    <div class="item" @click="toAppTrade">App交易</div>
    <div class="item" @click="toAboutUs">关于我们</div>
  </div>
</template>

<script lang="ts">
export default {
  props: ["data"],
  data() {
    return {};
  },
  methods: {
    toMitrade() {},
    toWebTrade() {},
    toAppTrade() {},
    toAboutUs() {},
  },
};
</script>

<style lang="less" scoped>
@import "./index.less";
</style>
