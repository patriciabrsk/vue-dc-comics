<template>
  <div id="footer">
    <div class="links-wrapper">
      <h4>DC Comics</h4>
      <nav>
        <ul>
          <li>
            <a href="#"></a>
          </li>
        </ul>
      </nav>
    </div>

    <div class="links-wrapper">
      <h4>DC</h4>
      <nav>
        <ul>
          <li>
            <a href="#"></a>
          </li>
        </ul>
      </nav>
    </div>

    <div class="links-wrapper">
      <h4>Sites</h4>
      <nav>
        <ul>
          <li>
            <a href="#"></a>
          </li>
        </ul>
      </nav>
    </div>

    <div class="links-wrapper">
      <h4>Shop</h4>
      <nav>
        <ul>
          <li>
            <a href="#"></a>
          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Footer",
  data() {
    return {
      DCComicsLinks: [
        {
          text: "Characters",
          url: "#",
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
        },
        {
          text: "Tv",
          url: "#",
        },
        {
          text: "Games",
          url: "#",
        },
        {
          text: "Collectibles",
          url: "#",
        },
        {
          text: "Videos",
          url: "#",
        },
        {
          text: "Fans",
          url: "#",
        },
        {
          text: "News",
          url: "#",
        },
        {
          text: "Shop",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_variables.scss";

div#footer {
  background-image: url("../assets/img/footer-bg.jpg");

  div.links-wrapper {
    display: flex;
    margin: 0 auto;
    width: 70%;

    h4 {
      color: white;
    }

    ul {
      display: flex;
      justify-content: space-evenly;

      li {
        list-style-type: none;
        text-transform: uppercase;
      }
    }
  }
}
</style>
