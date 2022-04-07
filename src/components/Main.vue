<template>
  <div>
    <!-- container-Jumbotron  -->
    <div class="container-bg_main-top">
      <div class="label-main-top">CURRENT SERIES</div>
    </div>
    <!-- container Comics  -->
    <div class="container-bg-main-bottom">
      <div class="content-dc-series">
        <SingoloFumetto
          v-for="(fumetto, index) in fumettiDc"
          :key="index"
          :fumetto="fumetto"
        />
      </div>
      <div class="container-button">
        <button>LOAD MORE</button>
      </div>
    </div>
  </div>
</template>

<script>
import fumettiDc from "@/assets/data-json/dc-comics";
import SingoloFumetto from "@/components/SingoloFumetto.vue";

export default {
  name: "Main_DC",
  data() {
    return {
      fumettiDc,
    };
  },
  components: {
    SingoloFumetto,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "src/variabili.scss";
.container-bg_main-top {
  background-image: url("@/assets/jumbotron.jpg");
  height: 380px;
  background-size: cover;
  position: relative;
  .label-main-top {
    background-color: $color-primary;
    padding: 10px 20px;
    color: white;
    position: absolute;
    bottom: -20px;
    left: 200px;
  }
}
.container-bg-main-bottom {
  background-color: $color-dark;
  .content-dc-series {
    width: $container-principal;
    margin: $margin-container;
    padding: 30px 0;
    display: flex;
    flex-wrap: wrap;
    gap: 15px;
  }
  .container-button {
    display: flex;
    justify-content: center;
    button {
      color: white;
      font-weight: bold;
      background-color: $color-primary;
      padding: 10px 30px;
      margin: 20px 0;
    }
  }
}
</style>
