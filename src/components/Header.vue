<template>
  <div id="header">
    <img src="../assets/img/dc-logo.png" alt="DC logo" />
    <ul>
      <li v-for="(link, index) in headerLinks" :key="index">
        <a :class="{ active: link.current }" :href="link.url">{{
          link.text
        }}</a>
      </li>
      <li>
        <a class="active" href="#">Comics</a>
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
@import "../assets/scss/partials/_variables.scss";

div#header {
  text-align: center;
  display: flex;
  margin: 20px auto;
  width: 70%;
  justify-content: space-between;
  font-size: 70%;

  img {
    width: 100px;
  }

  ul {
    display: flex;
    justify-content: space-evenly;

    li {
      list-style-type: none;
      text-transform: uppercase;
      display: flex;
      align-items: center;
      text-align: center;
      padding: 25px 10px;

      &:active,
      &.active {
        border-bottom: 5px solid #0082f9;
      }

      a {
        text-decoration: none;
        color: #303030;
      }
    }
  }
}
</style>
