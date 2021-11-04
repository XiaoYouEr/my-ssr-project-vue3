
<template>
  <div class="hot-news">
    <div class="left"><Card :data="newsData[0]" /></div>
    <div class="right">
      <div class="item one">
        <Card :data="newsData[1]" />
      </div>
      <div class="item one">
        <Card :data="newsData[2]" />
      </div>
      <div class="item one">
        <Card :data="newsData[3]" />
      </div>
      <div class="item one">
        <Card :data="newsData[4]" />
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Card from "./card.vue";
import Logo from "@/images/back.png";
export default {
  components: { Card },
  props: ["data"],
  data() {
    return {
      newsData: [
        {
          imgSrc: Logo,
          recommend: true,
          description:
            "9月海外市场的几个关键变量：疫情、通胀、美联储、财政9月海外市场的几个关键外市场的变量美联储、财政。。。。。。。。。。。。。。",
          author: "AAA",
          time: "2021-09-13 17:20 (GMT+8)",
        },
        {
          imgSrc: Logo,
          recommend: false,
          description:
            "9月海外市场的几个关键变量：疫情、通胀、美联储、财政9月海外市场的几个关键外市场的变量美联储、财政。。。。。。。。。。。。。。",
          author: "AAA",
          time: "2021-09-13 17:20 (GMT+8)",
        },
        {
          imgSrc: Logo,
          recommend: false,
          description:
            "9月海外市场的几个关键变量：疫情、通胀、美联储、财政9月海外市场的几个关键外市场的变量美联储、财政。。。。。。。。。。。。。。",
          author: "AAA",
          time: "2021-09-13 17:20 (GMT+8)",
        },
        {
          imgSrc: Logo,
          recommend: false,
          description:
            "9月海外市场的几个关键变量：疫情、通胀、美联储、财政9月海外市场的几个关键外市场的变量美联储、财政。。。。。。。。。。。。。。",
          author: "AAA",
          time: "2021-09-13 17:20 (GMT+8)",
        },
        {
          imgSrc: Logo,
          recommend: false,
          description:
            "9月海外市场的几个关键变量：疫情、通胀、美联储、财政9月海外市场的几个关键外市场的变量美联储、财政。。。。。。。。。。。。。。",
          author: "AAA",
          time: "2021-09-13 17:20 (GMT+8)",
        },
      ],
    };
  },
  methods: {},
};
</script>

<style lang="less" scoped>
@import "./index.less";
</style>
