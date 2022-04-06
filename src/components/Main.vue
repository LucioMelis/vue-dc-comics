<template>
  <div class="container-main">
    <div class="content">-- Content goes here --</div>
  </div>
</template>

<script>
export default {
  name: "Main_DC",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "src/variabili.scss";
.container-main {
  background-color: $color-dark;
  .content {
    width: $container-principal;
    margin: $margin-container;
    color: white;
    padding: 40px 0;
    font-weight: bold;
    font-size: 1.2rem;
  }
}
</style>
