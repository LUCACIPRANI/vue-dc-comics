<template>
  <div class="footer-Down">
    <span class="sign-up">
      SIGN UP NOW!
    </span>
    <span class="social-media">
      <div class="title">FOLLOW US &#160;</div>
      <ul>
        <li>
          <span
            class="footerIcon"
            v-for="(footerIcon, index) in footerIcons"
            :key="index"
          >
            <img
              :src="require(`../assets/img/${footerIcon.name}`)"
              alt="image"
            />
          </span>
        </li>
      </ul>
    </span>
  </div>
</template>

<script>
import * as footerIcons from "@/assets/data/features.js";
export default {
  name: "FooterDown",

  data() {
    return {
      footerIcons: footerIcons.footerIcons,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/style/mixins";
@import "@/style/vars";
@import "@/style/generals";

.footer-Down {
  // z-index: 3;
  background-color: #303030;
  height: 10vh;
  @include flexCenter();
}
.title {
  color: #1182f9;
  font-weight: bold;
  font-size: 90%;
}
.sign-up {
  border: 1px solid #1182f9;
  color: white;
  padding: 8px;
  font-size: 85%;
  margin-right: 210px;
  @include hoverIcons();
}
.social-media {
  @include flexCenter();
  img {
    height: 30px;
    width: 40px;
  }
}
</style>
