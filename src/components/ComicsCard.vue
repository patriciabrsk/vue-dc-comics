<template>
  <div id="card">
    <!-- <div class="card-wrapper"> -->
    <img :src="card.thumb" :alt="card.series" />
    <!-- </div> -->
    <h5>{{ card.series }}</h5>
  </div>
</template>

<script>
export default {
  name: "ComicsCard",
  props: {
    card: Object,
  },
};
</script>

<style lang="scss" scoped>
div#card {
  width: calc((100% / 6) - 2rem);
  margin-bottom: 1rem;

  // .card-wrapper {
  img {
    width: 100%;
    height: 120px;
    object-fit: cover;
  }
  // }
  h5 {
    text-transform: uppercase;
    font-size: 0.7rem;
    margin-top: 5px;
    color: white;
  }
}
</style>
