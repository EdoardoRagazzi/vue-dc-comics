<template>
  <div class="container">
    <img src="../assets/dc-logo.png" alt="" />
    <nav>
      <ul>
        <li
          v-for="(item, index) in navs"
          :key="index"
          :class="{ activeitem: item.current }"
        >
          <a :href="item.url" :class="{ activelink: item.current }">{{
            item.text
          }}</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
import NavsItems from "../data/Navs.js";

export default {
  name: "Header",
  data() {
    return {
      navs: NavsItems,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss" >
@import "../style/vars.scss";

.container {
  display: flex;
  justify-content: space-around;
  height: 115px;
  line-height: 100px;

  img {
    padding: 5px;
  }
  ul {
    padding-left: 50px;
    list-style: none;
    li {
      display: inline-block;
      padding: 5px;
      list-style: none;
      text-transform: $up;

      &:hover {
        color: blue;
        border-bottom: 5px solid blue;
        transition: 0.5s ease;
      }
      a {
        text-decoration: none;
        color: grey;
      }
    }
  }
}
</style>
