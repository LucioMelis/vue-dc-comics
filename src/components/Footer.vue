<template>
  <footer>
    <!-- ********footer top**********  -->
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
    <!-- ***********footer center***********  -->
    <div class="footer-center">
      <!-- container general footer center  -->
      <div class="container-footer-center">
        <!-- ***container List*** -->
        <div class="container-list">
          <!-- prima lista  -->
          <div>
            <h4>DC COMICS</h4>
            <ul>
              <li>Characters</li>
              <li>Comics</li>
              <li>Movies</li>
              <li>TV</li>
              <li>Games</li>
              <li>Videos</li>
              <li>News</li>
            </ul>
            <h4>SHOP</h4>
            <ul>
              <li>Shop DC</li>
              <li>Shop DC Collectibles</li>
            </ul>
          </div>
          <!-- seconda lista  -->
          <div>
            <h4>DC</h4>
            <ul>
              <li>Terms of Use</li>
              <li>Privacy policy(New)</li>
              <li>Ad Choices</li>
              <li>Advertising</li>
              <li>Jobs</li>
              <li>Subscriptions</li>
              <li>Talent Workshops</li>
              <li>CPSC Certificates</li>
              <li>Ratings</li>
              <li>Shop Help</li>
              <li>Contact Us</li>
            </ul>
          </div>
          <!-- terza lista  -->
          <div>
            <h4>SITES</h4>
            <ul>
              <li>DC</li>
              <li>MAD Magazine</li>
              <li>DC Kids</li>
              <li>DC Universe</li>
              <li>DC Power Visa</li>
            </ul>
          </div>
        </div>
        <!-- ***container background*** -->
        <div class="container-background"></div>
      </div>
    </div>
    <!-- ***********footer bottom***********  -->
    <div class="footer-bottom">
      <!-- container-footer-bottom  -->
      <div class="container-footer-bottom">
        <!-- container button  -->
        <div class="button-footer">
          <button>SIGN-UP NOW</button>
        </div>
        <!-- container img  -->
        <div class="follow-footer">
          <h4>FOLLOW US</h4>
          <div>
            <img src="../assets/footer-facebook.png" alt="Facebook" />
          </div>
          <div>
            <img src="../assets/footer-twitter.png" alt="Twitter" />
          </div>
          <div>
            <img src="../assets/footer-youtube.png" alt="YouTube" />
          </div>
          <div>
            <img src="../assets/footer-pinterest.png" alt="Pinterest" />
          </div>
          <div>
            <img src="../assets/footer-periscope.png" alt="Periscope" />
          </div>
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
.footer-center {
  background-image: url("../assets/footer-bg.jpg");
  background-size: cover;
  .container-footer-center {
    display: flex;
    width: $container-principal;
    margin: $margin-container;
    .container-list {
      display: flex;
      column-gap: 40px;
      padding: 30px 0;
      width: 50%;
      h4 {
        padding: 15px 0;
        color: white;
      }
      li {
        list-style-type: none;
        color: $text-color;
        padding: 2px 0;
        font-size: 11px;
      }
    }
  }
  .container-background {
    background-image: url("../assets/dc-logo-bg.png");
    width: 50%;
    background-repeat: no-repeat;
    background-position: center right;
    background-size: 450px;
  }
}
.footer-bottom {
  background-color: $color-bg-grey;
  .container-footer-bottom {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: $container-principal;
    margin: $margin-container;
    padding: 25px 0;
    .button-footer button {
      padding: 10px;
      border: 2px solid $color-primary;
      background-color: $color-bg-grey;
      color: white;
    }
    .follow-footer {
      display: flex;
      align-items: center;
      column-gap: 15px;
      h4 {
        color: $color-primary;
      }
      img {
        width: 25px;
      }
    }
  }
}
</style>