<template>
  <div id="content">
    <div class="wrapper flex">
      <h3>Content goes here</h3>
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
  background-color: #1c1c1c;
  width: 100%;

  div.wrapper {
    width: 70%;
    margin: 0 auto;
    align-items: center;
    height: 85px;

    h3 {
      color: white;
    }
  }
}
</style>
