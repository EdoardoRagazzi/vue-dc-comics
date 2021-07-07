<template>
  <div class="footer">
    <div class="image">
      <!-- <img src="../assets\dc-logo-bg.png" alt="" /> -->
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss" >
.footer {
  height: 300px;
  width: 100%;
  background-image: url(../assets/footer-bg.jpg);

  background-size: 100% 100%;
  background-repeat: no-repeat;
  .image {
    float: right;
    height: 300px;
    width: 300px;
    width: 45%;
    margin-right: 5%;
    background: transparent url("../assets/dc-logo-bg.png") no-repeat center;
    background-size: cover;
  }
}
</style>
