<template>
  <div id="shop-menu" class="flex">
    <div class="menu-links container flex">
      <div class="link flex">
        <a v-for="(link, index) in links" :key="index" class="flex">
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
          text: "DC merchandise",
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
@import "../assets/scss/style.scss";

div#shop-menu {
  background-color: $brandColor;
  gap: 1rem;
  justify-content: center;

  div.menu-links {
    justify-content: center;
    color: white;
    text-transform: uppercase;
    font-size: 0.7rem;

    div.link {
      justify-content: center;
      padding: 30px 0;
      gap: 3.5rem;

      a {
        margin: 0 auto;
        align-items: center;
        img {
          width: 45px;
          padding-right: 0.6rem;
        }
      }
    }
  }
}
</style>
