<template>
  <div id="app">
    <!-- header  -->
    <Header />
    <!-- content  -->
    <Content />
    <!-- blu icons  -->
    <Bluesection />
    <!-- footer top  -->
    <FooterTop />
    <!-- footer down  -->
    <FooterDown />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Content from "./components/Content.vue";
import Bluesection from "./components/Bluesection.vue";
import FooterTop from "./components/FooterTop.vue";
import FooterDown from "./components/FooterDown.vue";

export default {
  name: "App",
  components: {
    Header,
    Content,
    Bluesection,
    FooterTop,
    FooterDown,
  },
};
</script>

<style lang="scss">
@import "./style/generals";
@import "./style/vars";

#app {
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;

}
</style>
