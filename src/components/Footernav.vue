<template>
  <div class="footernav">
    <div class="btn">
      <button>Sign-up Now</button>
    </div>
    <div class="link">
      <h4>Follow Us</h4>
      <img src="@/assets/footer-facebook.png" alt="" />
      <img src="@/assets/footer-pinterest.png" alt="" />
      <img src="@/assets/footer-twitter.png" alt="" />
      <img src="@/assets/footer-youtube.png" alt="" />
      <img src="@/assets/footer-periscope.png" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Footernav",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss" >
@import "../style/commons.scss";
@import "../style/vars.scss";
.footernav {
  display: flex;
  text-transform: $up;
  justify-content: space-around;
  height: 100px;
  width: 100%;
  background-color: #303030;
  .btn {
    display: flex;
    align-self: center;
    button {
      height: 50px;
      width: 150px;
      font-size: 1em;
      font-weight: 600;
      color: white;
      text-transform: $up;
      border: 2px solid #0c7cec;
      background-color: #303030;
      &:hover {
        background-color: #0c7cec;
        cursor: pointer;
      }
    }
  }
  .link {
    line-height: 100px;
    h4 {
      font-weight: 900;
      font-size: 20px;
      display: inline-block;
      vertical-align: middle;
      padding-right: 50px;
      padding-bottom: 30px;
      color: #0c7cec;
    }
    img {
      padding-left: 15px;
      &:hover {
        cursor: pointer;
      }
    }
  }
}
</style>
