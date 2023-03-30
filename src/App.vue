<template>
  <BitcoinTicker />
  <nav class="navbar navbar-expand-lg bg-light">
    <div class="container-fluid">
      <a class="navbar-brand" href="/">
        <img
          src="./assets/logoAchilleus.png"
          alt="logo Achilleus"
          width="30"
          height="30"
          class="d-inline-block"
        />
        Achilleus Trading Bot
      </a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div
        class="collapse navbar-collapse"
        id="navbarSupportedContent"
      >
        <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a
              class="nav-link"
              aria-current="page"
              href="#"
              ><router-link to="/">Présentation</router-link></a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page"
              ><router-link to="/demo">Démo</router-link></a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page"
              ><router-link to="/faq">F.A.Q.</router-link></a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page"
              ><router-link to="/contact">Contact</router-link></a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page">
              <img
                src="./assets/telegram.png"
                alt="logo Achilleus"
                width="30"
                height="30"
                class="d-inline-block"
              />
            </a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
  <router-view />
</template>

<script>
import BitcoinTicker from "./components/BitcoinTicker.vue";

export default {
  name: "App",
  components: {
    BitcoinTicker,
  },
};
</script>

<style lang="scss">
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a:link {
    text-decoration: none;
  }

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
