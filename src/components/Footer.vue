<template>
  <div class="footer">
    <div class="listacolonne">
      <div class="col">
        <ul>
          <h4>DC Comics</h4>
          <li v-for="(comic, index) in Comics" :key="index">
            <a :href="comic.url">{{ comic.text }}</a>
          </li>
        </ul>
        <ul>
          <h4>DC Shop</h4>
          <li v-for="(shop, index) in Shop" :key="index">
            <a :href="shop.url">{{ shop.text }}</a>
          </li>
        </ul>
      </div>

      <div class="col">
        <ul>
          <h4>DC</h4>
          <li v-for="(dc, index) in Dc" :key="index">
            <a :href="dc.url">{{ dc.text }}</a>
          </li>
        </ul>
      </div>

      <div class="col">
        <ul>
          <h4>Sites</h4>
          <li v-for="(site, index) in Sites" :key="index">
            <a :href="site.url">{{ site.text }}</a>
          </li>
        </ul>
      </div>
    </div>
    <div class="image"></div>
  </div>
</template>

<script>
import listaComics from "@/data/listaComics.js";
import listaShop from "@/data/listaShop.js";
import listaDc from "@/data/listaDc.js";
import listaSites from "@/data/listaSites.js";
import listaIcons from "@/data/listaIcons.js";

export default {
  name: "Footer",
  data() {
    return {
      Comics: listaComics,
      Shop: listaShop,
      Dc: listaDc,
      Sites: listaSites,
      Icons: listaIcons.js,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../style/vars.scss";
.footer {
  height: 300px;
  width: 100%;
  background-image: url(../assets/footer-bg.jpg);

  background-size: 100% 100%;
  background-repeat: no-repeat;
  .listacolonne {
    display: inline-block;
    padding: 30px;
    color: white;
    font-weight: 900;
    text-transform: $up;
    font-size: 0.7em;
    .col {
      margin-right: 30px;
      display: inline-block;

      ul {
        list-style: none;
        li {
          text-align: left;
          a {
            text-decoration-line: none;
            color: #6a6a6a;
            text-align: left;
          }
        }
      }
    }
  }

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
