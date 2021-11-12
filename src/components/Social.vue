<template>
  <section class="socials">
    <div class="container d-flex">
      <div class="signup_button">
        <button>SIGN-UP NOW!</button>
      </div>
      <div class="social_links d-flex">
        <h4>FOLLOW US</h4>
        <a href="">
          <img src="../assets/img/footer-facebook.png" alt="" />
        </a>
        <a href="">
          <img src="../assets/img/footer-twitter.png" alt="" />
        </a>
        <a href="">
          <img src="../assets/img/footer-youtube.png" alt="" />
        </a>
        <a href="">
          <img src="../assets/img/footer-pinterest.png" alt="" />
        </a>
        <a href="">
          <img src="../assets/img/footer-periscope.png" alt="" />
        </a>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import "../assets/scss/variables.scss";
.socials {
  height: 120px;
  background-color: $social_bg_color;

  .container {
    height: 100%;
    justify-content: center;
    align-items: center;
  }
}

.signup_button {
  width: 50%;

  button {
    font-size: 1.1rem;
    color: $text_primary_color;
    background: none;
    border: 2px solid $highlight_primary_color;
    padding: 1rem;

    &:hover {
      cursor: pointer;
    }
  }
}

.social_links {
  justify-content: end;
  width: 50%;

  a {
    padding-left: 2rem;
  }

  h4 {
    line-height: 39px;
    color: $highlight_primary_color;
    font-size: 1.4rem;
  }
}
</style>