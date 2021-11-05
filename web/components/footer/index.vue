
<template>
  <div class="footer">
    <div class="nav">
      <div class="left">
        <img :src="logo" alt="" />
        <div>
          <div class="title">投资慧眼</div>
          <div class="des">为全球投资者提供全方位的优质专栏内容</div>
        </div>
      </div>
      <div class="right">
        <span class="item">热门</span>
        <span class="item">加密货币</span>
        <span class="item">美股</span>
        <span class="item">大宗商品</span>
        <span class="item">外汇</span>
        <span class="item">指数</span>
        <span class="item">其他</span>
      </div>
    </div>
    <div class="policy">
      <span class="item">隐私政策</span>
      <span class="item">产品披露声明</span>
      <span class="item">投诉流程</span>
      <span class="item">风险披露声明</span>
      <span class="item">客户协议</span>
    </div>
    <div class="description">
      <div class="section">
        风险警告：交易有可能导致您损失全部资金。场外衍生品交易并不适合所有人。敬请在使用我们的服务前仔细阅读我们的法律文件，并确保在交易前充分了解所涉及的风险。您并不实际拥有或持有任何相关基础资产。
      </div>
      <template v-if="!isCallapse">
        <div class="section">
          Mitrade不提供任何关于购买、持有或出售差价合约的建议、推荐或意见。我们提供的所有产品都是以全球资产作为基础的场外衍生品。Mitrade提供的所有服务仅基于执行交易指令。Mitrade
          不发行、购买或出售虚拟货币且并不是虚拟货币交易所。
        </div>
        <div class="section">
          Mitrade是由多家公司共同使用的业务品牌，透过以下公司进行运营： Mitrade
          Holding Ltd是本网站描述的或可提供使用的金融产品的发行人。Mitrade
          Holding
          Ltd获开曼群岛金融管理局（CIMA）授权并受其监管，SIB牌照号码为1612446，注册地址是：Buckingham
          Square, Phase II, 2nd Fl, 720 West Bay Road, George Town, Grand
          Cayman, Cayman Islands。 Mitrade Global Pty Ltd注册号码为ABN 90 149
          011 361, 澳大利亚金融服务牌照 (AFSL) 号码为 398528。
        </div>
        <div class="section">
          本网站资讯不针对美国，加拿大，日本，新西兰的居民；本网站资讯也不适合由于其发布或使用而违反当地法律或法规的任何国家或司法管辖区的任何人使用。敬请注意英语是我们服务所使用的主要语言，亦是我们所有合同文件中具有法律效力的语言。其他语言译本仅供参考，文译如与英文有歧义，概以英文为准。
        </div>
        <div class="ssl">
          SSL 安全通讯加密。© Mitrade版权所有， 保留一切权利。
        </div>
      </template>
      <div
        v-if="isCallapse"
        class="collapse on-close"
        @click="onChangeCollapse"
      >
        展开
      </div>
      <div v-else class="collapse on-open" @click="onChangeCollapse">折叠</div>
    </div>
    <div class="top-wrap">
      <div class="top" @click="scrollToTop"></div>
    </div>
  </div>
</template>

<script lang="ts">
import Logo from "@/images/logo.png";
export default {
  props: ["data"],
  data() {
    return {
      logo: Logo,
      isCallapse: true,
    };
  },
  methods: {
    onChangeCollapse() {
      this.isCallapse = !this.isCallapse;
    },
    scrollToTop() {
      window.scrollTo({ top: 0, behavior: "smooth" });
    },
  },
};
</script>

<style lang="less" scoped>
@import "./index.less";
</style>
