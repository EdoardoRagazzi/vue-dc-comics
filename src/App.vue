
<template>
  <div id="app">
    <Header />
    <Jumbotron />
    <Products />
    <Footer />
    <Footernav />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Jumbotron from "./components/Jumbotron.vue";
import Products from "./components/Products.vue";
import Footer from "./components/Footer.vue";
import Footernav from "./components/Footernav.vue";

export default {
  name: "App",
  components: {
    Header,
    Jumbotron,
    Products,
    Footer,
    Footernav,
  },
};
</script>

<style lang="scss">
@import "style/commons.scss";
@import "style/vars.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100vh;
}
</style>
