<template>
  <div id="content">
    <div id="jumbotron"></div>
    <div class="cards-wrapper flex">
      <div class="container">
        <h4 class="tag text-uppercase">Current series</h4>
        <div class="cards flex">
          <ComicsCard
            v-for="(card, index) in cards"
            :key="index"
            :card="card"
          />
        </div>
        <div class="button flex">
          <button class="btn text-uppercase">Load More</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import cards from "../assets/dc-comics.json";
import ComicsCard from "./ComicsCard.vue";

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Content",
  components: { ComicsCard },
  data() {
    return {
      cards,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/style.scss";

div#content {
  div#jumbotron {
    height: 42vh;
    background-image: url("../assets/img/jumbotron.jpg");
    background-size: cover;
  }

  div.cards-wrapper {
    background-color: #1c1c1c;
    width: 100%;
    align-items: center;

    div.container {
      position: relative;
      padding: 3rem 0;
      h4.tag {
        color: white;
        padding: 0.3rem 0.9rem;
        background-color: $brandColor;
        position: absolute;
        top: 0;
        transform: translateY(-50%);
      }
      .cards {
        flex-wrap: wrap;
        justify-content: center;
      }
      div.button {
        justify-content: center;

        .btn {
          background-color: $brandColor;
          font-size: 0.7rem;
          font-weight: 400;
          color: white;
          border: none;
          padding: 0.6rem 2.5rem;
          &:hover {
            cursor: pointer;
          }
        }
      }
    }
  }
}
</style>
