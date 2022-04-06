<template>
  <header>
    <div class="container-header">
      <div class="container-header-logo">
        <img src="../assets/dc-logo.png" alt="Dc-Logo" />
      </div>
      <div class="container-nav">
        <ul>
          <li><a href="#">CHARACTERS</a></li>
          <li><a href="#">COMICS</a></li>
          <li><a href="#">MOVIES</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">GAMES</a></li>
          <li><a href="#">COLLECTIBLES</a></li>
          <li><a href="#">VIDEO</a></li>
          <li><a href="#">FANS</a></li>
          <li><a href="#">NEWS</a></li>
          <li><a href="#">SHOP</a></li>
        </ul>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header_DC",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container-header {
  width: 70%;
  margin: auto;
  background-color: $color-primary;
}
</style>
