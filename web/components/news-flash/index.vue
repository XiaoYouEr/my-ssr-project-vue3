
<template>
  <div class="news-flash">
    <div class="header">
      <div class="title">新闻快讯</div>
      <div class="more">查看更多</div>
    </div>
    <div class="news-content">
      <div class="tabs">
        <div
          :class="`tab ${currentTab === 1 ? 'active' : ''}`"
          @click="changeTab(1)"
        >
          加密货币
        </div>
        <div
          :class="`tab ${currentTab === 2 ? 'active' : ''}`"
          @click="changeTab(2)"
        >
          美股
        </div>
        <div
          :class="`tab ${currentTab === 3 ? 'active' : ''}`"
          @click="changeTab(3)"
        >
          大宗商品
        </div>
        <div
          :class="`tab ${currentTab === 4 ? 'active' : ''}`"
          @click="changeTab(4)"
        >
          外汇
        </div>
        <div
          :class="`tab ${currentTab === 5 ? 'active' : ''}`"
          @click="changeTab(5)"
        >
          指数
        </div>
      </div>
      <div class="card-wrap">
        <div class="card">
          <div class="time">2021-09-13 17:20 (GMT+8)</div>
          <div class="des">
            疫情、通胀、美联储、财政9月海外市场的几个关键变量：疫情、通胀、美联储、财政疫情、通胀、美联储、财政具体点。。。。。。。。。。。。。
          </div>
          <div class="tags">
            <div class="tag">美联储</div>
            <div class="tag">风险偏好</div>
            <div class="tag">美元/瑞郎</div>
          </div>
        </div>
        <div class="card">
          <div class="time">2021-09-13 17:20 (GMT+8)</div>
          <div class="des">
            疫情、通胀、美联储、财政9月海外市场的几个关键变量：疫情、通胀、美联储、财政疫情、通胀、美联储、财政具体点。。。。。。。。。。。。。
          </div>
          <div class="tags">
            <div class="tag">美联储</div>
            <div class="tag">风险偏好</div>
            <div class="tag">美元/瑞郎</div>
          </div>
        </div>
        <div class="card">
          <div class="time">2021-09-13 17:20 (GMT+8)</div>
          <div class="des">
            疫情、通胀、美联储、财政9月海外市场的几个关键变量：疫情、通胀、美联储、财政疫情、通胀、美联储、财政具体点。。。。。。。。。。。。。
          </div>
          <div class="tags">
            <div class="tag">美联储</div>
            <div class="tag">风险偏好</div>
            <div class="tag">美元/瑞郎</div>
          </div>
        </div>
        <div class="card">
          <div class="time">2021-09-13 17:20 (GMT+8)</div>
          <div class="des">
            疫情、通胀、美联储、财政9月海外市场的几个关键变量：疫情、通胀、美联储、财政疫情、通胀、美联储、财政具体点。。。。。。。。。。。。。
          </div>
          <div class="tags">
            <div class="tag">美联储</div>
            <div class="tag">风险偏好</div>
            <div class="tag">美元/瑞郎</div>
          </div>
        </div>
        <div class="card">
          <div class="time">2021-09-13 17:20 (GMT+8)</div>
          <div class="des">
            疫情、通胀、美联储、财政9月海外市场的几个关键变量：疫情、通胀、美联储、财政疫情、通胀、美联储、财政具体点。。。。。。。。。。。。。
          </div>
          <div class="tags">
            <div class="tag">美联储</div>
            <div class="tag">风险偏好</div>
            <div class="tag">美元/瑞郎</div>
          </div>
        </div>
      </div>
    </div>
    <div class="from">来源：FXStreet</div>
  </div>
</template>

<script lang="ts">
export default {
  props: ["data"],
  data() {
    return {
      currentTab: 1,
    };
  },
  methods: {
    changeTab(tab: number) {
      this.currentTab = tab;
    },
  },
};
</script>

<style lang="less" scoped>
@import "./index.less";
</style>
