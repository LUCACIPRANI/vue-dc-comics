<template>
  <div id="app">
    <Header />
    <Jumbotron />
    <BoxComics />
    <Bluesection />
    <FooterTop />
    <FooterDown />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Jumbotron from "./components/Jumbotron.vue";
import BoxComics from "./components/BoxComics.vue";
import Bluesection from "./components/Bluesection.vue";
import FooterTop from "./components/FooterTop.vue";
import FooterDown from "./components/FooterDown.vue";

export default {
  name: "App",
  components: {
    Header,
    Jumbotron,
    BoxComics,
    Bluesection,
    FooterTop,
    FooterDown,
  },
};
</script>

<style lang="scss">
@import "./style/generals";
@import "./style/vars";

// #app {

// }
</style>
