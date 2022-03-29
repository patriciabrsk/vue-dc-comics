<template>
  <div id="footer-nav">
    <div class="nav-wrapper container flex">
      <div class="sign-up">
        <a href="#">Sign-up now!</a>
      </div>

      <div class="social-wrapper flex">
        <div class="follow">
          <p>Follow us</p>
        </div>
        <div class="icons flex">
          <img src="../assets/img/footer-facebook.png" alt="FB logo" />
          <img src="../assets/img/footer-twitter.png" alt="Twitter logo" />
          <img src="../assets/img/footer-youtube.png" alt="YT logo" />
          <img src="../assets/img/footer-pinterest.png" alt="Pinterest logo" />
          <img src="../assets/img/footer-periscope.png" alt="Gmaps logo" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Footer-Nav",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

div#footer-nav {
  background-color: #303030;
  color: white;

  div.nav-wrapper {
    align-items: center;
    justify-content: space-between;
    height: 12vh;

    div.sign-up {
      a {
        text-decoration: none;
        color: white;
        padding: 10px;
        border: 2px solid $brandColor;
        text-transform: uppercase;
        font-size: 0.8rem;
        font-weight: 300;
      }
    }

    div.social-wrapper {
      align-items: center;
      gap: 1rem;
      justify-content: space-between;

      div.follow p {
        text-transform: uppercase;
        font-weight: 600;
        color: $brandColor;
      }

      div.icons {
        align-items: center;
        gap: 0.8rem;
      }
    }
  }
}
</style>
