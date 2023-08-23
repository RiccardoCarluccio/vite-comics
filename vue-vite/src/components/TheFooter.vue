<script>
  export default {
    data() {
      return {
        dcComicsLinks: [
          { name: "characters", path: "/" },
          { name: "comics", path: "/" },
          { name: "movies", path: "/" },
          { name: "tv", path: "/" },
          { name: "games", path: "/" },
          { name: "videos", path: "/" },
          { name: "news", path: "/" },
        ],
        shop: [
          { name: "shop dc", path: "/" },
          { name: "shop dc collectibles", path: "/" },
        ],
        dc: [
          { name: "terms of use", path: "/" },
          { name: "privacy policy (new)", path: "/" },
          { name: "ad choices", path: "/" },
          { name: "advertising", path: "/" },
          { name: "jobs", path: "/" },
          { name: "subscription", path: "/" },
          { name: "talent workshop", path: "/" },
          { name: "cpsc certificates", path: "/" },
          { name: "ratings", path: "/" },
          { name: "shop help", path: "/" },
          { name: "contact us", path: "/" },
        ],
        sites: [
          { name: "dc", path: "/" },
          { name: "mad magazine", path: "/" },
          { name: "dc kids", path: "/" },
          { name: "dc universe", path: "/" },
          { name: "dc power visa", path: "/" },
        ],
      };
    },
  };
</script>

<template>
  <footer>
    <div id="footer-background" class="container-fluid">
      <div class="container">
        <div class="d-flex justify-content-between align-items-center">
          <div class="d-flex">
            <div class="d-flex flex-wrap flex-column gap-5">
              <h3 class="text-white text-uppercase fw-bold">
                dc comics
              </h3>
              <ul class="nav nav-pills d-flex flex-column">
                <li class="nav-item" v-for="link in dcComicsLinks">
                  <a href="#" class="nav-link text-white" :class="{ active: link.name === 'Prodotti' }">
                    {{ link.name }}
                  </a>
                </li>
              </ul>

              <h3 class="text-white text-uppercase fw-bold">
                shop
              </h3>
              <ul class="nav nav-pills d-flex flex-column">
                <li class="nav-item" v-for="link in shop">
                  <a href="#" class="nav-link text-white" :class="{ active: link.name === 'Prodotti' }">
                    {{ link.name }}
                  </a>
                </li>
              </ul>
            </div>

            <div>
              <h3 class="text-white text-uppercase fw-bold">
                dc
              </h3>
              <ul class="nav nav-pills d-flex flex-column">
                <li class="nav-item" v-for="link in dc">
                  <a href="#" class="nav-link text-white" :class="{ active: link.name === 'Prodotti' }">
                    {{ link.name }}
                  </a>
                </li>
              </ul>
            </div>

            <div>
              <h3 class="text-white text-uppercase fw-bold">
                site
              </h3>
              <ul class="nav nav-pills d-flex flex-column">
                <li class="nav-item" v-for="link in sites">
                  <a href="#" class="nav-link text-white" :class="{ active: link.name === 'Prodotti' }">
                    {{ link.name }}
                  </a>
                </li>
              </ul>
            </div>
          </div>

          <img src="../../vue-dc-comics-1/img/dc-logo-bg.png" alt="DC Logo Background">
        </div>
      </div>

      <div class="container-fluid bg-dark">
        <div class="container d-flex justify-content-between align-items-center">
          <div>
            <button type="button" id="footer-button" class="btn btn-outline-primary text-uppercase text-white border-2">sign-up now!</button>
          </div>
          <div class="d-flex justify-content-end align-items-center gap-3 py-3">
            <h4 class="text-uppercase text-primary">follow us</h4>
            <img src="../../vue-dc-comics-1/img/footer-facebook.png" alt="">
            <img src="../../vue-dc-comics-1/img/footer-periscope.png" alt="">
            <img src="../../vue-dc-comics-1/img/footer-pinterest.png" alt="">
            <img src="../../vue-dc-comics-1/img/footer-twitter.png" alt="">
            <img src="../../vue-dc-comics-1/img/footer-youtube.png" alt="">
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>
  #footer-background {
    background-image: url("../../vue-dc-comics-1/img/footer-bg.jpg");
    background-size: cover;
  }

  #footer-button {
    border-radius: 0;
  }

  footer h3 {
    margin-bottom: -10px;
  }

  footer a {
      font-size: 14px;
      margin: -7px;
    }
</style>