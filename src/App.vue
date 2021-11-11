<template>
  <div id="app">
    <SiteHeader />
    <!-- /#site_header -->
    <main id="site_main">
      <section class="content_section container">
        <h2>-- Content goes here --</h2>
      </section>
      <!-- /.content_section -->
      <section class="content_index">
        <ul class="index_options d-flex container">
          <li>
            <a href="#">
              <div class="index_link">
                <img src="./assets/img/buy-comics-digital-comics.png" alt="" />
                <h5>DIGITAL COMICS</h5>
              </div>
            </a>
          </li>
          <li>
            <a href="#">
              <div class="index_link">
                <img src="./assets/img/buy-comics-merchandise.png" alt="" />

                <h5>DC MERCHANDISE</h5>
              </div>
            </a>
          </li>
          <li>
            <a href="#">
              <div class="index_link">
                <img src="./assets/img/buy-comics-subscriptions.png" alt="" />

                <h5>SUBSCRIPTION</h5>
              </div>
            </a>
          </li>
          <li>
            <a href="#">
              <div class="index_link">
                <img
                  src="./assets/img/buy-comics-shop-locator.png"
                  alt=""
                  class="locator_logo"
                />

                <h5>COMIC SHOP LOCATOR</h5>
              </div>
            </a>
          </li>
          <li>
            <a href="#">
              <div class="index_link">
                <img src="./assets/img/buy-dc-power-visa.svg" alt="" />

                <h5>DC POWER VISA</h5>
              </div>
            </a>
          </li>
        </ul>
      </section>
      <!-- /.content_index -->
    </main>
    <!-- /#site_main -->
    <footer id="site_footer">
      <section class="ext_links"></section>
      <!-- /.ext_links -->
      <section class="socials"></section>
      <!-- /.socials -->
    </footer>
    <!-- /#site_footer -->
  </div>
</template>

<script>
import SiteHeader from "./components/SiteHeader.vue";
export default {
  name: "App",
  components: {
    SiteHeader,
  },
};
</script>

<style lang="scss">
@import "./assets/scss/common.scss";
@import "./assets/scss/variables.scss";
#site_main {
  background-color: $content_bg_color;

  .content_section {
    color: $text_primary_color;
    padding: 3rem 0px;
  }

  .content_index {
    background-color: $highlight_primary_color;
    padding: 3rem 0px;

    .index_options {
      justify-content: space-around;
      align-items: center;

      h5 {
        color: $text_primary_color;
        font-weight: normal;
        padding-left: 10px;
      }
    }

    .index_link {
      display: flex;
      align-items: center;
    }

    .locator_logo {
      width: 30px;
    }

    img {
      width: 40px;
    }
  }
}
</style>
