<template>
  <div class="container">
    <span class="cards-section">
      <img :src="boxProp.thumb" :alt="boxProp.type" />
      <h5>{{ boxProp.series.toUpperCase() }}</h5>
    </span>
  </div>
</template>

<script>
export default {
  name: "CardsBoxComics",
  props: ["boxProp"],
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/style/generals";
@import "@/style/mixins";
@import "@/style/vars";

.container {
  margin: 0 auto;
  width: 73%;
  margin-top: 30px;
}
.cards-section {
  @include centerColumn();
  height: 180px;
  width: calc(100% / 6);
  float: left;
  text-align: center;

  img {
    height: 70%;
    width: 150px;
    object-fit: cover;
  }
}

h5 {
  font-weight: 500;
  font-size: 70%;
  color: white;
  padding-top: 1em;
}
</style>
