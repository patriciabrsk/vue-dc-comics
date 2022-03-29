<template>
  <div id="content">
    <div id="jumbotron"></div>
    <div class="cards-wrapper flex">
      <div class="container">
        <h3>Content goes here</h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Content",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/style.scss";

div#content {
  div#jumbotron {
    height: 30vh;
    background-image: url("../assets/img/jumbotron.jpg");
    background-size: cover;
  }

  div.cards-wrapper {
    background-color: #1c1c1c;
    width: 100%;
    align-items: center;
    height: 85px;

    h3 {
      color: white;
    }
  }
}
</style>
