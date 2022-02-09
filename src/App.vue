<template>
    <Header />
    <Brand />
    <Audience />
    <DesignPhoto />
    <Testimonials />
    <Gallery />
    <Footer />
</template>

<script>
  import Header from "./components/Header.vue";
  import Brand from "./components/Brand.vue";
  import Audience from "./components/Audience.vue";
  import DesignPhoto from "./components/Design_Photo.vue";
  import Testimonials from "./components/Testimonials.vue";
  import Gallery from "./components/Gallery.vue";
  import Footer from "./components/Footer.vue"

  export default {
    name: 'App',
    components: {
      Header,Brand,
      Audience,DesignPhoto,
      Testimonials,Gallery,
      Footer
    }
  }
</script>

<style>
  *,
  *::after,
  *::before {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  :root {
    --clr-soft-red: hsl(7, 99%, 70%);
    --clr-yellow: hsl(51, 100%, 49%);
    /* (graphic design text) */
    --clr-dark-desaturated-cyan: hsl(167, 40%, 24%);
    /* (photography text) */
    --clr-dark-blue: hsl(198, 62%, 26%);
    /* (footer) */
    --clr-dark-moderate-cyan: hsl(168, 34%, 41%);

    --very-dark-desaturated-blue: hsl(212, 27%, 19%);
    --very-dark-grayish-blue: hsl(213, 9%, 39%);
    --dark-grayish-blue: hsl(232, 10%, 55%);
    --grayish-blue: hsl(210, 4%, 67%);
    --white: hsl(0, 0%, 100%);

    /* Fonts */
    --font-primary: 'Barlow', sans-serif;
    --font-secondary: 'Fraunces', serif;
  }

  body {
    font-size: 18px;
    height: 100vh;
    font-family: var(--font-primary);
    font-weight: 600;
    overflow-x: hidden;
  }

  a {
    text-decoration: none;
  }

  ul {
    list-style: none;
  }

  img {
    width: 100%;
    display: block;
  }

  section h1 {
    color: var(--very-dark-desaturated-blue);
    font-family: var(--font-secondary);
    font-weight: 900;
  }

  .btn {
    font-family: var(--font-secondary);
    font-weight: 900;
    font-size: 23px;
    text-decoration: underline;
    text-decoration-color: var(--clr-soft-red);
  }
</style>