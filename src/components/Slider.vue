<template>
  <div class="slider">
    <div
      v-for="(item, index) in myJson"
      :key="index"
      class="col-2 d-inline-block"
    >
      <CardSlider :slider="item" />
    </div>
  </div>
</template>

<script>
import json from "@/json/dc-comics.json";
import CardSlider from "@/components/CardSlider.vue";

export default {
  name: "Slider",
  components: {
    CardSlider,
  },
  data() {
    return {
      listCharacter: [],
      myJson: json,
    };
  },
  created() {
    this.getCharacters();
  },
  methods: {
    getCharacters() {
      this.listCharacter = this.myJson;
      console.log(this.listCharacter);
    },
  },
};
</script>

<style scoped lang="scss">
.slider {
  background-color: #303030;
  width: 100%;
  padding: 50px;
}
</style>