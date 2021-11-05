
<template>
  <div class="hot-articles">
    <div class="header">
      <div class="title">热门文章</div>
      <div class="switch">
        <span
          :class="`item ${currentTab === 1 ? 'active' : ''}`"
          @click="changeTab(1)"
          >阅读更多</span
        >
        <span
          :class="`item ${currentTab === 2 ? 'active' : ''}`"
          @click="changeTab(2)"
          >最新发布</span
        >
      </div>
    </div>
    <div class="news-content">
      <div class="card" v-for="(item, index) in list" :key="index">
        <img class="left" :src="item.head" alt="" />
        <div class="right">
          <div class="title">{{ item.title }}</div>
          <div class="des">{{ item.description }}</div>
          <div class="bottom">
            <div class="info">
              <span class="author">
                {{ item.author }}
              </span>
              <span class="time">
                {{ item.time }}
              </span>
              <span class="view">
                {{ item.view }}
              </span>
            </div>
            <div class="tags">
              <div class="tag" v-for="(tag, i) in item.tags" :key="i">
                <div class="tag">{{ tag }}</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="foot"></div>
  </div>
</template>

<script lang="ts">
import Head from "@/images/back.png";
export default {
  props: ["data"],
  data() {
    return {
      currentTab: 1,
      list: [
        {
          head: Head,
          author: "Lucy",
          time: "1小时前",
          view: "1000",
          tags: ["美股", "美联储", "美元走势"],
          title:
            "9月海外市场的几个关键变量：疫情、通胀、美联储、财政9月海外市场的几个关键变量：疫情、通胀、美联储、财政疫、美联储、财政xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
          description:
            "9月海外市场的几个关键变量：疫情、通胀、美联储、财政9月海外市场的几个关键变量：疫情、通胀、美联储、财政疫、美联储、财政xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
        },
        {
          head: Head,
          author: "Lucy",
          time: "1小时前",
          view: "1000",
          tags: ["美股", "美联储", "美元走势"],
          title:
            "9月海外市场的几个关键变量：疫情、通胀、美联储、财政9月海外市场的几个关键变量：疫情、通胀、美联储、财政疫、美联储、财政xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
          description:
            "9月海外市场的几个关键变量：疫情、通胀、美联储、财政9月海外市场的几个关键变量：疫情、通胀、美联储、财政疫、美联储、财政xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
        },
        {
          head: Head,
          author: "Lucy",
          time: "1小时前",
          view: "1000",
          tags: ["美股", "美联储", "美元走势"],
          title:
            "9月海外市场的几个关键变量：疫情、通胀、美联储、财政9月海外市场的几个关键变量：疫情、通胀、美联储、财政疫、美联储、财政xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
          description:
            "9月海外市场的几个关键变量：疫情、通胀、美联储、财政9月海外市场的几个关键变量：疫情、通胀、美联储、财政疫、美联储、财政xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
        },
        {
          head: Head,
          author: "Lucy",
          time: "1小时前",
          view: "1000",
          tags: ["美股", "美联储", "美元走势"],
          title:
            "9月海外市场的几个关键变量：疫情、通胀、美联储、财政9月海外市场的几个关键变量：疫情、通胀、美联储、财政疫、美联储、财政xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
          description:
            "9月海外市场的几个关键变量：疫情、通胀、美联储、财政9月海外市场的几个关键变量：疫情、通胀、美联储、财政疫、美联储、财政xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
        },
        {
          head: Head,
          author: "Lucy",
          time: "1小时前",
          view: "1000",
          tags: ["美股", "美联储", "美元走势"],
          title:
            "9月海外市场的几个关键变量：疫情、通胀、美联储、财政9月海外市场的几个关键变量：疫情、通胀、美联储、财政疫、美联储、财政xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
          description:
            "9月海外市场的几个关键变量：疫情、通胀、美联储、财政9月海外市场的几个关键变量：疫情、通胀、美联储、财政疫、美联储、财政xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
        },
        {
          head: Head,
          author: "Lucy",
          time: "1小时前",
          view: "1000",
          tags: ["美股", "美联储", "美元走势"],
          title:
            "9月海外市场的几个关键变量：疫情、通胀、美联储、财政9月海外市场的几个关键变量：疫情、通胀、美联储、财政疫、美联储、财政xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
          description:
            "9月海外市场的几个关键变量：疫情、通胀、美联储、财政9月海外市场的几个关键变量：疫情、通胀、美联储、财政疫、美联储、财政xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
        },
      ],
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
