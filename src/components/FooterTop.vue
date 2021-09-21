<template>
  <div class="background">
    <div class="left-side">
      <div class="column">
        <h5>DC COMICS</h5>
        <ul>
          <li>Characters</li>
          <li>Comics</li>
          <li>Movies</li>
          <li>TV</li>
          <li>Games</li>
          <li>Videos</li>
          <li>News</li>
        </ul>
        <h5>SHOPS</h5>
        <ul>
          <li>Shop DC</li>
          <li>Shop DC Collectibles</li>
        </ul>
      </div>
      <div class="column">
        <h5>DC</h5>
        <ul>
          <li>Terms Of Use</li>
          <li>Provacy policy (New)</li>
          <li>Ad Choices</li>
          <li>Advertising</li>
          <li>Jobs</li>
          <li>Subscriptions</li>
          <li>Talent Workshops</li>
          <li>CPCS Certificates</li>
          <li>Ratings</li>
          <li>Shop Help</li>
          <li>Contacts Us</li>
        </ul>
      </div>
      <div class="column">
        <h5>SITES</h5>
        <ul>
          <li>DC</li>
          <li>MAD Magazine</li>
          <li>DC Kids</li>
          <li>DC Universe</li>
          <li>DC Power Visa</li>
        </ul>
      </div>
    </div>
    <div class="right-side"></div>
  </div>
</template>

<script>
export default {
  name: "FooterTop",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/style/mixins";
@import "@/style/vars";

.background {
  @include flexStart();
  background-image: url("../assets/img/footer-bg.jpg");
  height: 36vh;
}
.left-side {
  float: left;
}
.column {
  float: left;
  text-align: left;
  padding-right: 15px;
  h5 {
    color: white;
    margin: 8px 0;
  }
  ul li {
    font-size: 60%;
    color: #888580;
    line-height: 1.6em;
    list-style: none;
    text-decoration: none;
  }
}
.right-side {
  background-image: url("../assets/img/dc-logo-bg.png");
  margin-left: 25%;
  background-size: contain;
  background-repeat: no-repeat;
  height: 420px;
  width: 450px;
}
</style>
