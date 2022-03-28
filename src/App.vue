<template>
  <div id="app">
    <!-- Header -->
    <Header />

    <!-- Main -->
    <Content />

    <!-- Shop Menu -->
    <ShopMenu />

    <!-- Footer -->
    <Footer />

    <!-- Footer Nav -->
    <FooterNav />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Content from "./components/Content.vue";
import ShopMenu from "./components/ShopMenu.vue";
import Footer from "./components/Footer.vue";
import FooterNav from "./components/FooterNav.vue";

export default {
  name: "App",
  components: {
    Header,
    Content,
    ShopMenu,
    Footer,
    FooterNav,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
