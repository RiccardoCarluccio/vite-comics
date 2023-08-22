<script>
  export default {
    data() {
      return {
        navLinks: [
          { name: "characters", path: "/" },
          { name: "comics", path: "/" },
          { name: "movies", path: "/" },
          { name: "tv", path: "/" },
          { name: "games", path: "/" },
          { name: "collectibles", path: "/" },
          { name: "videos", path: "/" },
          { name: "fans", path: "/" },
          { name: "news", path: "/" },
          { name: "shop", path: "/" },
        ],
      };
    },
  };
</script>

<template>
  <header>
    <img src="../../vue-dc-comics-1/img/dc-logo.png" alt="DC Logo">

    <ul class="nav nav-pills">
      <li class="nav-item" v-for="link in navLinks">
        <a href="#" class="nav-link" :class="{ active: link.name === 'Prodotti' }">
          {{ link.name }}
        </a>
      </li>
    </ul>
  </header>
</template>

<style lang="scss" scoped>

</style>