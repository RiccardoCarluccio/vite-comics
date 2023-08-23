<script>
  import Card from "../components/Card.vue";
  import ComicsDatabase from "../../dc-comics.json";

  export default {
  data() {
    return {
      ComicsDatabase,
    };
  },
  components: {
    Card,
  },
};
</script>

<template>
  <div class="row">

  </div>

  <div id="jumbotron" class="container-fluid"></div>

  <div class="container-fluid bg-black d-flex justify-content-center align-items-center">
    <div class="row container text-white py-5 gy-5">
        <div v-for="Comic in ComicsDatabase" class="col-2">
          <TheCard :img-src="Comic.thumb" :series-title="Comic.series"></TheCard>
        </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  #jumbotron {
    background-image: url("../../vue-dc-comics-1/img/jumbotron.jpg");
    height: 300px;
    background-size: cover;
  }
</style>