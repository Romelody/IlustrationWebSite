<template>
  <div id="Eachpost">
    <div class="">
      <div class="post-container">
        <img :src="img" alt="img" />
        <div class="acctions">
          <div class="like">
            <img :src="emptyHeart" alt="" />
            <p>0</p>
          </div>
          <div class="comment">
            <img :src="emptyHeart" alt="" />
            <p>0</p>
          </div>
          <div class="share">
            <img :src="emptyHeart" alt="" />
            <p>0</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
// import art01 from "../../public/img/art-01.jpg";
import emptyHeart from "../../public/img/line-heart.svg";
export default {
  props: {
    img: String
  },
  data: function() {
    return {
      // art01: art01,
      emptyHeart: emptyHeart
    };
  }
};
</script>
<style lang="scss">
#Eachpost {
  .post-container {
    padding: 20px;
    background: #f4f4f4;
    border-radius: 15px;
    /* width: 33%; */
    img {
      border-radius: 10px;
      width: 100%;
      height: 100%;
    }
  }
  .acctions {
    padding-top: 20px;
    display: flex;
    justify-content: space-between;
    .like {
      display: flex;
    }
    .comment {
      display: flex;
    }
    .share {
      display: flex;
    }
    img {
      width: 20px;
      margin-right: 10px;
    }
  }
}
</style>
