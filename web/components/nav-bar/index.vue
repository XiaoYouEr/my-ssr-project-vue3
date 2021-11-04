
<template>
  <div class="nav-bar">
    <div class="left">
      <div class="logo-wrap">
        <img class="logo" :src="logo" />
        <div class="title">投资慧眼</div>
      </div>
      <div class="item">热门</div>
      <div class="item">加密货币</div>
      <div class="item">美股</div>
      <div class="item">大宗商品</div>
      <div class="item">外汇</div>
      <div class="item">指数</div>
      <div class="item">其他</div>
    </div>
    <div class="search-wrap">
      <input class="search-input" :value="searchValue" placeholder="搜索" />
    </div>
  </div>
</template>

<script lang="ts">
import Logo from "@/images/logo.png";
export default {
  props: ["data"],
  data() {
    return {
      searchValue: "",
      logo: Logo,
    };
  },
  methods: {},
};
</script>

<style lang="less" scoped>
@import "./index.less";
</style>
