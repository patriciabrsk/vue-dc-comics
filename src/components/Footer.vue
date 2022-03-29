<template>
  <div id="footer">
    <div class="footer-wrapper flex">
      <div class="links-wrapper container flex">
        <div class="links-list">
          <h4>DC Comics</h4>
          <nav>
            <ul>
              <li v-for="(link, index) in dcComicsLinks" :key="index">
                <a :href="link.url">{{ link.text }}</a>
              </li>
            </ul>
          </nav>

          <div>
            <h4>Shop</h4>
            <nav>
              <ul>
                <li v-for="(link, index) in shopLinks" :key="index">
                  <a :href="link.url">{{ link.text }}</a>
                </li>
              </ul>
            </nav>
          </div>
        </div>

        <div class="links-list">
          <h4>DC</h4>
          <nav>
            <ul>
              <li v-for="(link, index) in dcLinks" :key="index">
                <a :href="link.url">{{ link.text }}</a>
              </li>
            </ul>
          </nav>
        </div>

        <div class="links-list">
          <h4>Sites</h4>
          <nav>
            <ul>
              <li v-for="(link, index) in sitesLinks" :key="index">
                <a :href="link.url">{{ link.text }}</a>
              </li>
            </ul>
          </nav>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Footer",
  data() {
    return {
      dcComicsLinks: [
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
      shopLinks: [
        {
          text: "Shop DC",
          url: "#",
        },
        {
          text: "Shop DC Collectibles",
          url: "#",
        },
      ],
      dcLinks: [
        {
          text: "Terms of Use",
          url: "#",
        },
        {
          text: "Privacy policy (New)",
          url: "#",
        },
        {
          text: "Ad Choices",
          url: "#",
        },
        {
          text: "Advertising",
          url: "#",
        },
        {
          text: "jobs",
          url: "#",
        },
        {
          text: "Subscriptions",
          url: "#",
        },
        {
          text: "Talent Workshops",
          url: "#",
        },
        {
          text: "Fans",
          url: "#",
        },
        {
          text: "CPSC Certificates",
          url: "#",
        },
        {
          text: "Shop Help",
          url: "#",
        },
        {
          text: "Contact Us",
          url: "#",
        },
      ],
      sitesLinks: [
        {
          text: "DC",
          url: "#",
        },
        {
          text: "MAD Magazine",
          url: "#",
        },
        {
          text: "Ad Choices",
          url: "#",
        },
        {
          text: "Advertising",
          url: "#",
        },
        {
          text: "jobs",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

div#footer {
  background-image: url("../assets/img/footer-bg.jpg");

  div.footer-wrapper {
    font-size: 0.8rem;
    justify-content: space-around;

    div.links-wrapper {
      background-image: url("../assets/img/dc-logo-bg.png");
      background-repeat: no-repeat;
      background-size: 48%;
      background-position: center right;

      div.links-list {
        padding: 22px 0;
        margin-right: 15px;
        h4 {
          color: white;
          text-transform: uppercase;
          margin-bottom: 0.6rem;
        }

        ul {
          padding-left: 0;
          margin-bottom: 0.6rem;

          li {
            list-style-type: none;

            a {
              text-decoration: none;
              font-size: 0.7rem;
              color: #797979;
            }
          }
        }
      }
    }
  }
}
</style>
