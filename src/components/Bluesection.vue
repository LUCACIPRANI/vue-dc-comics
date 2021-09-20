<template>
  <div class="blue-section">
    <nav>
      <ul>
        <li>
          <div class="elements" v-for="(icon, index) in icons" :key="index">
            <div class="img">
              <img :src="require(`../assets/img/${icon.image}`)" alt="image" />
            </div>
            <div class="text">
              {{ icon.name }}
            </div>
          </div>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
import * as icons from "@/assets/data/features.js";
export default {
  name: "BlueSection",

  data() {
    return {
      icons: icons.icons,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/style/mixins";
@import "@/style/vars";

.blue-section {
  height: 15vh;
  color: white;
  background-color: #1182f9;
  @include center();
}
nav ul li {
  padding: 10px;
  @include center();
}
.text {
  padding: 0 15px;
}
.elements{
  @include center();
  font-size: 70%;
  padding: 10px;
  img{
    height: 40px;
    width: 40px;
  }
}

</style>
