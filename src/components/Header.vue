<template>
  <div id="header" class="flex">
    <img src="../assets/img/dc-logo.png" alt="DC logo" />
    <ul class="flex">
      <li
        v-for="(link, index) in headerLinks"
        :key="index"
        class="flex text-uppercase"
      >
        <a :class="{ active: link.current }" :href="link.url">{{
          link.text
        }}</a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Header",
  data() {
    return {
      headerLinks: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "Tv",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

div#header {
  align-items: center;
  height: 12vh;
  margin: 0 auto;
  width: 70%;
  justify-content: space-between;
  font-size: 70%;
  font-weight: 600;

  img {
    width: 60px;
    height: 60px;
  }

  ul {
    justify-content: space-evenly;

    li {
      list-style-type: none;
      align-items: center;
      text-align: center;
      height: 12vh;
      padding: 10px;
      border-bottom: 3px solid transparent;

      &:active,
      &.active {
        border-bottom: 3px solid $brandColor;
      }

      a {
        text-decoration: none;
        color: #303030;

        &:active,
        &:hover,
        &.active {
          color: $brandColor;
        }
      }
    }
  }
}
</style>
