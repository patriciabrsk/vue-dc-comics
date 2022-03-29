<template>
  <div id="shop-menu">
    <div class="menu-links">
      <div class="link">
        <a v-for="(link, index) in links" :key="index">
          <img :src="require(`@/assets/img/${link.img}`)" :alt="link.text" />
          <span>{{ link.text }}</span>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "ShopMenu",
  data() {
    return {
      links: [
        {
          text: "Digital Comics",
          img: "buy-comics-digital-comics.png",
        },
        {
          text: "DC merchandising",
          img: "buy-comics-merchandise.png",
        },
        {
          text: "Subscription",
          img: "buy-comics-subscriptions.png",
        },
        {
          text: "Comic shop locator",
          img: "buy-comics-shop-locator.png",
        },
        {
          text: "DC Power Visa",
          img: "buy-dc-power-visa.svg",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_variables.scss";

div#shop-menu {
  background-color: $brandColor;
  display: flex;
  gap: 1rem;
  justify-content: center;

  div.menu-links {
    width: 70%;
    display: flex;
    justify-content: center;
    color: white;
    text-transform: uppercase;
    font-size: 0.7rem;

    div.link {
      display: flex;
      align-items: center;
      text-align: center;
      margin: 0 auto;
      padding: 22px 0 22px;

      a {
        display: flex;
        margin: 0 auto;
        align-items: center;
        img {
          width: 35px;
          padding-right: 0.5rem;
        }
        span {
          padding-right: 3rem;
        }
      }
    }
  }
}
</style>
