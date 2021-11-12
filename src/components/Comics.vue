<template>
  <div class="comic">
    <div class="comic_image">
      <img :src="image" alt="" />
    </div>
    <h3 class="title">{{ series }}</h3>
  </div>
</template>

<script>
export default {
  props: {
    image: String,
    series: String,
  },
};
</script>

<style lang="scss">
.comic {
  margin: 1rem 0%;
  .comic_image {
    width: 200px;
    height: 190px;
    overflow: hidden;

    &:hover {
      cursor: pointer;
    }
  }
  .title {
    font-size: 1rem;
    width: 200px;
    margin: 1rem 0%;
  }
}
</style>