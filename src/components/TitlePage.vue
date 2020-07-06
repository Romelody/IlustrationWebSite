<template>
  <div id="Title" class="hello">
    <div class="container">
      <h1 class="TitlePage">{{ msg }}</h1>
      <h3 class="AditionalInformation">
        I made this site to show my art, if you want to see more please follow
        me on Instagram!
      </h3>
      <img src="" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "TitlePage",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#Title {
  .TitlePage {
    text-align: left;
  }
  .AditionalInformation {
    text-align: left;
    width: 40%;
  }
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
