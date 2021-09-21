<template>
  <div class="Jumbotron-section"></div>
</template>

<script>
import * as boxes from "@/assets/data/features.js";
export default {
  name: "Jumbotron",

  data() {
    return {
      boxes: boxes.boxes,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/style/mixins";
@import "@/style/vars";

.Jumbotron-section {
  background-color: #1c1c1c;
  height: 40vh;
  color: white;
  @include flexStart();
  background-image: url("../assets/img/jumbotron.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  // &:before{
  //   content: '--->';
  // }
  // &:after{
  //   content: '<---';
  // }
}
</style>
