<template>
  <div class="box-section">
    <div>
      <span class="h2">CURRENT SERIES</span>
    </div>
    <div>
      <CardsBoxComics
        v-for="(box, index) in boxes"
        :key="index"
        :boxProp="box"
      />
    </div>

    <div class="load">
      <span class="h3">
        LOAD MORE
      </span>
    </div>
  </div>
</template>

<script>
import CardsBoxComics from "@/components/CardsBoxComics.vue";
import * as features from "../assets/data/features.js";

export default {
  name: "BoxComics",
  components: {
    CardsBoxComics,
  },
  data() {
    return {
      boxes: features.boxes,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/style/generals";
@import "@/style/mixins";
@import "@/style/vars";

.box-section {
  padding-bottom: 15px;
  background-color: #1c1c1c;
  height: 500px;
  position: relative;

  .h2 {
    @include btn();
    margin-left: 190px;
    font-size: 110%;
  }
  .load {
    position: absolute;
    top: 90%;
    left: 50%;
    transform: translate(-50%, -50%);

    .h3 {
      @include btn();
      font-size: 70%;
      text-align: center;
    }
  }
}
</style>
