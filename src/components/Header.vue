<template>
  <header>
    <div class="container py-3">
      <nav class="d-flex align-items-center justify-content-between">
        <a href="#"><img src="/images/logo.svg" alt="logo" /></a>

        <ul class="d-md-flex gap-3 align-items-center d-none d-md-block">
          <li v-for="list in lists" :key="list.id"><a href="#">{{list.name}}</a></li>
          <li><a class="active" href="#">Contact</a></li>
        </ul>

        <i @click="toggleBtn" role="button" class="d-block d-md-none fa-solid fs-2 fa-bars text-white"></i>
      </nav>

      <h1 class="text-center text-white text-uppercase mt-5">
        We are <br />
        creatives
      </h1>

      <img src="/images/icon-arrow-down.svg" alt="arrow-down" class="arrow" />

      <div v-if="toggle" class="menu-mobile">
        <ul class="text-center d-flex flex-column gap-4">
          <li v-for="list in lists" :key="list.id"><a href="#">{{list.name}}</a></li>
          <li><a href="#" class="active">Contact</a></li>
        </ul>
      </div>
    </div>
  </header>
</template>

<script>
export default {
    data() {
        return {
            toggle: false,
            lists: [
              {name: "About"},
              {name: "Services"},
              {name: "Projects"},
            ]
        }
    },

    methods: {
        toggleBtn() {
            this.toggle = !this.toggle;
        }
    }
};
</script>

<style scoped>
header {
  background-image: url("/images/mobile/image-header.jpg");
  background-size: cover;
  background-position: center;
  height: 100vh;
  position: relative;
}

header h1 {
  font-family: var(--font-secondary);
  font-weight: 900;
  font-size: 50px;
}

.menu-mobile {
  background-color: var(--white);
  position: absolute;
  width: 90%;
  margin: 0 auto;
  top: 3em;
  left: 0;
  transform: translateX(6%);
  font-size: 16px;
  border-radius: 10px;
  margin-top: 1em;
}

.menu-mobile ul > li > a {
  color: var(--grayish-blue) !important;
}

.menu-mobile ul {
  width: 100%;
  margin: 1em auto;
  padding: 0;
}

.menu-mobile ul .active {
  background-color: var(--clr-yellow);
  color: var(--clr-dark-desaturated-cyan) !important;
  padding: 12px 24px;
  border-radius: 10px;
}

.arrow {
  width: 50px;
  display: block;
  margin: 0 auto;
  margin-top: 4em;
}

@media only screen and (min-width: 800px) {
  header {
    background-image: url("/images/desktop/image-header.jpg");
  }

  header nav ul li a {
    color: var(--white);
  }

  header nav ul .active {
    color: var(--very-dark-desaturated-blue) !important;
    padding: 9px 24px;
    background: var(--white);
    border-radius: 10px;
    font-family: var(--font-secondary);
  }
}
</style>