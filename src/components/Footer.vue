<template>
  <footer>
    <!-- footer top  -->
    <div class="footer-top">
      <!-- container footer-top  -->
      <div class="container-footer-top">
        <!-- container singola card  -->
        <div class="container-card">
          <img
            src="../assets/buy-comics-digital-comics.png"
            alt="digi-comics"
          />
          <p>DIGITAL COMICS</p>
        </div>
        <div class="container-card">
          <img src="../assets/buy-comics-merchandise.png" alt="merchandise" />
          <p>DC MERCHANDISE</p>
        </div>
        <div class="container-card">
          <img
            src="../assets/buy-comics-subscriptions.png"
            alt="subscriptions"
          />
          <p>SUBSCRIPTION</p>
        </div>
        <div class="container-card">
          <img src="../assets/buy-comics-shop-locator.png" alt="locator" />
          <p>COMIC SHOP LOCATOR</p>
        </div>
        <div class="container-card">
          <img src="../assets/buy-dc-power-visa.svg" alt="power-visa" />
          <p>DC POWER VISA</p>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer_DC",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "src/variabili.scss";
.footer-top {
  background-color: #0282f9;
  .container-footer-top {
    width: $container-principal;
    margin: $margin-container;
    display: flex;
    justify-content: space-around;
    color: white;
    padding: 50px 0;
    & div:last-child img {
      width: 50px;
    }
    .container-card {
      display: flex;
      align-items: center;
      column-gap: 10px;
      img {
        height: 50px;
      }
      p {
        font-size: 11px;
      }
    }
  }
}
</style>