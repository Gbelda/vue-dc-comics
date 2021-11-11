<template>
  <div id="app">
    <SiteHeader />
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
</style>
