<template>
  <div class="cardi">
    <img :src="slider.thumb" class="card-img-top" />

    <p>
      {{ slider.series }} <br />
      {{ slider.price }} <br />
      {{ slider.type }}
    </p>
  </div>
</template>

<script>
export default {
  name: "CardSlider",
  props: ["slider"],
};
</script>

<style scoped lang="scss">
@import "@/style/commons.scss";
@import "@/style/vars.scss";
.cardi {
  padding: 30px;
  height: 200px;
  text-align: center;
  color: white;
  img {
    margin: auto;
    height: 150px;
    width: 150px;
  }
}
</style>



