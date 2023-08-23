<script>
  export default {
  props: {
    imgSrc: String,

    comicTitle: {
      type: String,
      required: true,
    },
  },
};
</script>

<template>
  <img :src="imgSrc" alt="" />
  <div class="pt-3 text-uppercase">{{ comicTitle }}</div>
</template>

<style lang="scss" scoped>

</style>