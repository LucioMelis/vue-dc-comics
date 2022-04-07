<template>
  <div class="card-fumetto">
    <img :src="fumetto.thumb" alt="fumetto" />
    <p>{{ fumetto.series }}</p>
  </div>
</template>

<script>
export default {
  name: "SingoloFumetto",
  props: {
    fumetto: Object,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "src/variabili.scss";
.card-fumetto {
  width: calc(100% / 6 - 15px * 5 / 6);
  img {
    width: 100%;
  }
  p {
    color: white;
    font-size: 12px;
    padding: 10px 0;
  }
}
</style>
