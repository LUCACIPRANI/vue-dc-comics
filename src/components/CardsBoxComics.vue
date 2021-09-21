<template>
  <div class="cards-section">
    <img :src="boxProp.thumb" :alt="boxProp.type" />
    <h5>{{ boxProp.series }}</h5>
  </div>
</template>

<script>
export default {
  name: "CardsBoxComics",
  props: ['boxProp'],
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/style/mixins";
@import "@/style/vars";

.cards-section {
  height: 200px;
  width: 50px;
  border: 1px solid red;
  float: left;
  @include center();
}
h5 {
  font-weight: 500;
  color: white;
}
</style>
