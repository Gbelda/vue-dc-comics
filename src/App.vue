<template>
  <div id="app">
    <SiteHeader />
    <!-- /#site_header -->

    <SiteMain />
    <!-- /#site_main -->

    <footer id="site_footer">
      <FooterIndex />
      <!-- /.ext_links -->

      <Social />
      <!-- /.socials -->
    </footer>
    <!-- /#site_footer -->
  </div>
</template>
 
<script>
import SiteHeader from "./components/SiteHeader.vue";
import SiteMain from "./components/SiteMain.vue";
import FooterIndex from "./components/FooterIndex.vue";
import Social from "./components/Social.vue";

export default {
  name: "App",
  components: {
    SiteHeader,
    SiteMain,
    FooterIndex,
    Social,
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap");
@import "./assets/scss/common.scss";
</style>
