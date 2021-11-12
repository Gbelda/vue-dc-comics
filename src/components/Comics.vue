<template>
  <div>
    <img :src="image" alt="" />
  </div>
  <h3>{{ series }}</h3>
</template>

<script>
export default {
  props: {
    image: String,
    series: String,
  },
};
</script>

<style>
</style>