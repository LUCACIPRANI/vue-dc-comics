<template>
  <div class="content-section">
    <h2>--> Content goes here ---</h2>
  </div>
</template>

<script>
export default {
  name: 'Content',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import "@/style/mixins";
@import "@/style/vars";

.content-section{
  background-color: #1C1C1C;
  height: 12vh;
  color: white;
  @include flexStart();
}

</style>
