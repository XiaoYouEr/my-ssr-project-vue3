<template>
  <div class="container">
    <PageHeader />
    <NavBar />
    <div class="content">
      <router-view />
      <Footer />
    </div>
  </div>
</template>

<script lang="ts">
// 在这里可以进行一些全局组件的注册逻辑
import PageHeader from "@/components/header/index.vue";
import NavBar from "@/components/nav-bar/index.vue";
import Footer from "@/components/footer/index.vue";

export default {
  components: {
    PageHeader,
    NavBar,
    Footer,
  },
  props: ["data"],
  data() {
    return {
      count: 0,
    };
  },
};
</script>
