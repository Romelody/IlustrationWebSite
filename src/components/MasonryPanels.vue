<template>
  <div id="MasonryPanels">
    <div class="container">
      <div
        v-masonry="containerId"
        transition-duration="0.3s"
        item-selector=".item"
        gutter="5"
      >
        <Eachpost
          v-masonry-tile
          class="item"
          v-for="item in blocks"
          :key="item.id"
          :img="item.img"
          :class="item.class"
        />
      </div>
      <!-- <Eachpost /> -->
    </div>
  </div>
</template>
<script>
import Eachpost from "./Eachpost.vue";
import Vue from "vue";
import { VueMasonryPlugin } from "vue-masonry";
import art01 from "../../public/img/art-01.jpg";
Vue.use(VueMasonryPlugin);

export default {
  components: {
    Eachpost
  },
  data: function() {
    return {
      blocks: [
        {
          id: 0,
          img: art01,
          class: "item"
        },
        {
          id: 1,
          img: art01,
          class: "item2"
        },
        {
          id: 2,
          img: art01,
          class: "item"
        },
        {
          id: 3,
          img: art01,
          class: "item"
        }
      ]
    };
  }
};
</script>

<style>
.item {
  width: 33%;
  margin-bottom: 10px;
}
.item2 {
  width: 66%;
  margin-bottom: 10px;
}
</style>
