<template>
  <div id="app">
    <TitlePage msg="All my Illustrations" />
    <MasonryPanels />
  </div>
</template>

<script>
import TitlePage from "./components/TitlePage.vue";
import MasonryPanels from "./components/MasonryPanels.vue";

export default {
  name: "App",
  components: {
    TitlePage,
    MasonryPanels
  }
};
</script>

<style lang="scss">
* {
  box-sizing: border-box;
}
.container {
  width: 90%;
  margin: 0 auto;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
