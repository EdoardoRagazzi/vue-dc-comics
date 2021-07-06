<template>
  <div class="jumbotron">
    <h3>--> Content Goes Here</h3>
  </div>
</template>

<script>
export default {
  name: "Jumbotron",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss" >
.jumbotron {
  background-color: black;
  height: 200px;
  width: 100%;
  color: white;
  font-size: 9vh;
  h3 {
    float: left;
    padding: 40px;
  }
}
</style>
