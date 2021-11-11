<template>
  <div id="app">
    <header id="site_header">
      <nav class="nav_bar d-flex container">
        <div class="logo">
          <img src="./assets/img/dc-logo.png" alt="" />
        </div>
        <div class="nav_links">
          <ul class="d-flex">
            <li>
              <a href="#">
                <h5>CHARACTERS</h5>
              </a>
            </li>
            <li>
              <a href="#">
                <h5>COMICS</h5>
              </a>
            </li>
            <li>
              <a href="#">
                <h5>MOVIES</h5>
              </a>
            </li>
            <li>
              <a href="#">
                <h5>TV</h5>
              </a>
            </li>
            <li>
              <a href="#">
                <h5>GAMES</h5>
              </a>
            </li>
            <li>
              <a href="#">
                <h5>COLLECTIBLES</h5>
              </a>
            </li>
            <li>
              <a href="#">
                <h5>VIDEOS</h5>
              </a>
            </li>
            <li>
              <a href="#">
                <h5>FANS</h5>
              </a>
            </li>
            <li>
              <a href="#">
                <h5>NEWS</h5>
              </a>
            </li>
            <li>
              <a href="#">
                <h5>SHOP</h5>
              </a>
            </li>
          </ul>
        </div>
      </nav>
    </header>
    <!-- /#site_header -->
    <main id="site_main">
      <section class="content_section"></section>
      <!-- /.content_section -->
      <section class="content_index"></section>
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
export default {
  name: "App",
  components: {},
};
</script>

<style lang="scss">
@import "./assets/scss/common.scss";
@import "./assets/scss/variables.scss";
#site_header {
  .logo {
    img {
      width: 80px;
    }
  }
  .nav_bar {
    align-items: center;
    justify-content: space-between;
  }
  .nav_links {
    ul {
      list-style: none;
      li {
        padding-left: 1.5rem;
        a {
          text-decoration: none;
          color: $nav_text_primary_color;

          h5 {
            padding: 3rem 0px;
            border-bottom: 5px solid transparent;
            &:hover {
              border-bottom-color: $highlight_primary_color;
              color: $highlight_primary_color;
            }
          }
        }
      }
    }
  }
}
</style>
