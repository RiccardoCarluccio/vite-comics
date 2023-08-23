<script>
  import TheHeader from "./components/TheHeader.vue";
  import TheFooter from "./components/TheFooter.vue";
  import TheMain from "./components/TheMain.vue";
  import TheRealMain from "./components/TheRealMain.vue";

  export default {
    components: {
      TheHeader,
      TheMain,
      TheFooter,
      TheRealMain,
    },
    data() {
      return {};
    },
  };
</script>

<template>
  <TheHeader></TheHeader>

  <TheRealMain></TheRealMain>

  <TheMain></TheMain>

  <TheFooter></TheFooter>
</template>

<style lang="scss">
  @use "./styles/general.scss";
</style>
