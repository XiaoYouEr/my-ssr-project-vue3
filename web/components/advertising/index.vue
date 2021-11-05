
<template>
  <div class="advertising">
    <img :src="advertising" alt="" />
  </div>
</template>

<script lang="ts">
import Advertising from "@/images/back.png";
export default {
  props: ["data"],
  data() {
    return {
      advertising: Advertising,
    };
  },
  methods: {},
};
</script>

<style lang="less" scoped>
@import "./index.less";
</style>
