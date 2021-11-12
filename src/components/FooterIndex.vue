<template>
  <section class="ext_links d-flex">
    <div class="d-flex container main_footer">
      <div class="index_container d-flex">
        <div class="index_section">
          <h4>DC COMICS</h4>
          <ul id="dc_comics">
            <li><a href="#">Characters</a></li>
            <li><a href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">News</a></li>
          </ul>
          <h4>SHOP</h4>
          <ul>
            <li><a href="#">Shop DC</a></li>
            <li><a href="#">Shop DC Collectibles</a></li>
          </ul>
        </div>
        <div class="index_section">
          <h4>DC</h4>
          <ul>
            <li><a href="#">Terms Of Use</a></li>
            <li><a href="#">Privacy Policy (New)</a></li>
            <li><a href="#">Ad Choices</a></li>
            <li><a href="#">Advertising</a></li>
            <li><a href="#">Jobs</a></li>
            <li><a href="#">Subscriptions</a></li>
            <li><a href="#">Talent Workshops</a></li>
            <li><a href="#">CPSC Certificates</a></li>
            <li><a href="#">Ratings</a></li>
            <li><a href="#">Shop Help</a></li>
            <li><a href="#">Contact Us</a></li>
          </ul>
        </div>
        <div class="index_section">
          <h4>SITES</h4>
          <ul>
            <li><a href="#">DC</a></li>
            <li><a href="#">MAD Magazine</a></li>
            <li><a href="#">DC Kids</a></li>
            <li><a href="#">DC Universe</a></li>
            <li><a href="#">DC Power Visa</a></li>
          </ul>
        </div>
      </div>
      <!-- <div class="footer_dc_logo"></div> -->
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import "../assets/scss/variables.scss";

.ext_links {
  background-image: url(../assets/img/footer-bg.jpg);
  height: 400px;

  .index_container {
    padding: 4rem 0px;
    width: 100%;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position: right;
    background-size: 590px;
    height: 400px;

    .index_section {
      padding-right: 2rem;
    }
  }

  .main_footer {
    justify-content: space-between;
  }

  .footer_dc_logo {
    width: 100%;
    height: 400px;
  }

  h4 {
    color: $text_primary_color;
    font-size: 1.3rem;
  }

  h4,
  #dc_comics {
    padding-bottom: 1rem;
  }

  li {
    a {
      font-size: 0.9rem;
      color: rgb(136, 136, 136);
    }
  }
}
</style>