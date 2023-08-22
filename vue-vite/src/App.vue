<script>
  import TheHeader from "./components/TheHeader.vue";
  import TheFooter from "./components/TheFooter.vue";

  export default {
    components: {
      TheHeader,
      TheFooter,
    },
    data() {
      return {};
    },
  };
</script>

<template>
  <TheHeader></TheHeader>

  <main>
    <div class="container text-center">

    </div>
  </main>

  <TheFooter></TheFooter>
</template>

<style lang="scss">
  @use "./styles/general.scss";
</style>
