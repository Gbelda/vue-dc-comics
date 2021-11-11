<template>
  <div id="app">
    <SiteHeader />
    <!-- /#site_header -->
    <SiteMain />
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
import SiteMain from "./components/SiteMain.vue";
export default {
  name: "App",
  components: {
    SiteHeader,
    SiteMain,
  },
};
</script>

<style lang="scss">
@import "./assets/scss/common.scss";
@import "./assets/scss/variables.scss";
</style>
