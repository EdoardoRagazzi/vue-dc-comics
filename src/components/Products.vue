<template>
  <div class="products">
    <div class="container">
      <ul>
        <li v-for="(link, index) in links" :key="index">
          <img :src="iconSrc(link.img)" :alt="link.alt" />
          <span class="icon-caption">{{ link.caption }}</span>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Products",
  data() {
    return {
      links: [
        {
          img: "buy-comics-digital-comics.png",
          alt: "DC Digital Comics icon",
          caption: "Digital Comics",
        },
        {
          img: "buy-comics-merchandise.png",
          alt: "DC Merchandise icon",
          caption: "Merchandise",
        },
        {
          img: "buy-comics-subscriptions.png",
          alt: "DC Subscription icon",
          caption: "Subscription",
        },
        {
          img: "buy-comics-shop-locator.png",
          alt: "DC Shop Locator icon",
          caption: "Comic Shop Locator",
        },
        {
          img: "buy-dc-power-visa.svg",
          alt: "DC Power Visa con",
          caption: "DC Power Visa",
        },
      ],
    };
  },

  methods: {
    iconSrc(icon) {
      return require("../assets/" + icon);
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.products {
  background-color: #0282f9;
  height: 100px;
  width: 100%;
  color: white;
  font-size: 3vh;
  .container {
    height: 100%;
    align-items: center;
  }
  ul {
    height: 100%;
    list-style: none;
    display: flex;
    justify-content: space-between;
    align-items: center;
    li {
      font-size: 1rem;
      cursor: pointer;
      align-content: center;

      img {
        height: 40px;
        width: auto;
        vertical-align: middle;
      }
      .icon-caption {
        margin-left: 10px;
        text-transform: uppercase;
      }
    }
  }
}
</style>



