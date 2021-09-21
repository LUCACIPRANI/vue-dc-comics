<template>
  <div class="box-section">
    <span class="h2">CURRENT SERIES</span>

    <div>
      <CardsBoxComics
        v-for="(box, index) in boxes"
        :key="index"
        :boxProp="box"
      />
    </div>
    
  <div class="Load">
    <span class="h3">
      LOAD MORE
    </span>
  </div>
  </div>
</template>

<script>
import CardsBoxComics from "@/components/CardsBoxComics.vue";
import boxes from "@/assets/data/features.js";

export default {
  name: "BoxComics",
  components: {
    CardsBoxComics,
  },
  data() {
    return {
      boxes: boxes,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/style/mixins";
@import "@/style/vars";

.box-section {
  height: 10vh;
  background-color: #1c1c1c;
  .h2 {
    @include btn();
    margin-left: 190px;
  }
  .Load{
    @include center();
    .h3{
    @include btn();
    font-size: 70%;
    text-align: center;
  }
  }
  
}
</style>
