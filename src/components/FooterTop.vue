<template>
  <div class="background">
    <div class="footer-top">
      <div class="column">
        <h4>DC COMICS</h4>
        <ul>
          <li>Characters</li>
          <li>Comics</li>
          <li>Movies</li>
          <li>TV</li>
          <li>Games</li>
          <li>Videos</li>
          <li>News</li>
        </ul>
        <h4>SHOPS</h4>
        <ul>
          <li>Shop DC</li>
          <li>Shop DC Collectibles</li>
        </ul>
      </div>
      <div class="column">
        <h4>DC</h4>
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
        <h4>SITES</h4>
        <ul>
          <li>DC</li>
          <li>MAD Magazine</li>
          <li>DC Kids</li>
          <li>DC Universe</li>
          <li>DC Power Visa</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterTop",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.background{
  background-image: "@/assets/images/bg.jpg";
}
.footer-top {
  width: 35%;
}
.column {
  float: left;
  h4 {
    color: white;
  }
  ul li {
    font-size: 80%;
  }
}
</style>
