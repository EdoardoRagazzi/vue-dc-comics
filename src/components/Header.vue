<template>
  <div class="container">
    <img src="../assets/dc-logo.png" alt="" />
    <ul class="nav">
      <li class="nav-item">Characters</li>
      <li class="nav-item">Comics</li>
      <li class="nav-item">Movies</li>
      <li class="nav-item">Tv</li>
      <li class="nav-item">Games</li>
      <li class="nav-item">Collectibles</li>
      <li class="nav-item">Videos</li>
      <li class="nav-item">Fan</li>
      <li class="nav-item">News</li>
      <li class="nav-item">Shop</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss" >
@import "../style/vars.scss";

.container {
  display: flex;
  justify-content: space-around;
  height: 100px;
  line-height: 100px;

  img {
    padding: 5px;
  }
  ul {
    padding-left: 50px;
  }
  li {
    display: inline-block;
    padding: 8px;

    text-transform: $up;
    height: 100%;
    &:hover {
      color: blue;
      border-bottom: 5px solid blue;
    }
  }
}
</style>
