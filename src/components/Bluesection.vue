<template>
  <div class="blue-section">

     <nav>
      <ul>
        <span v-for="(icons, index) in icons" :key="index">
          <img :src="'@/assets/images' + 'buy-comics-digital-comics.png'" 
          alt="image">
        <li v-for="(icon, index) in icons" :key="index">
            {{ icon.name }}
        </li>
        </span>
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
      icons: icons.icons
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/style/mixins";
@import "@/style/vars";

.blue-section{
  height: 18vh;
  color: white;
  background-color: #1182F9;
}
nav ul{
  display: flex;
  flex-direction: row;
  align-items: end;
  justify-content: center;
}

</style>
