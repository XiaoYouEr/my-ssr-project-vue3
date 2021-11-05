
<template>
  <div>
    <!-- <Search /> -->
    <HotNews />
    <!-- <template v-if="indexData">
      <Slider :data="indexData[0].components" />
      <Rectangle :data="indexData[1].components" />
    </template>
    <template v-else>
      <img
        src="https://gw.alicdn.com/tfs/TB1v.zIE7T2gK0jSZPcXXcKkpXa-128-128.gi"
        class="loading"
      />
    </template> -->
    <div class="center">
      <div class="left-recommend">
        <HotTopic />
        <NewsFlash />
        <Advertising />
      </div>
      <div class="right-recommend">
        <HotArticles />
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { mapState } from "vuex";
import Slider from "@/components/slider/index.vue";
import Rectangle from "@/components/rectangle/index.vue";
import Search from "@/components/search/index.vue";
import HotNews from "@/components/hot-news/index.vue";
import HotArticles from "@/components/hot-articles/index.vue";
import HotTopic from "@/components/hot-topic/index.vue";
import NewsFlash from "@/components/news-flash/index.vue";
import Advertising from "@/components/advertising/index.vue";

export default defineComponent({
  components: {
    Slider,
    Rectangle,
    Search,
    HotNews,
    HotArticles,
    HotTopic,
    NewsFlash,
    Advertising,
  },
  computed: {
    ...mapState({
      indexData: (state) => {
        console.log("state", state.indexStore);
        return state.indexStore?.data;
      },
    }),
  },
});
</script>

<style>
@import "./index.less";
</style>
