<template>
  <div class="header">
    <nav>
      <img alt="DC logo" src="@/assets/img/dc-logo.png" />
      <ul>
        <li v-for="(feature, index) in features" :key="index">
          <a :class="feature.current ? 'active' : null" href="feature.url">
            {{ feature.name }}
            <!-- <span class="blue-bar"></span> -->
          </a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
import * as features from "@/assets/data/features.js";
export default {
  name: "Header",

  data() {
    return {
      features: features.features,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
// importing SCSS rules;
@import "@/style/mixins";
@import "@/style/vars";

.header {
  background-color: white;
  color: #000;
  font-weight: 500;
  padding: 10px 0;
  nav {
    @include flexCenter();
    ul {
      @include flexCenter();
      li {
        padding: 1rem;
        font-size: 65%;
        list-style: none;
        a {
          list-style: none;
          text-decoration: none;
          color: #736A7F;

          &:hover,
          &.active {
            color: $activeColor;
          }
        }
      }
    }
  }
}
</style>
