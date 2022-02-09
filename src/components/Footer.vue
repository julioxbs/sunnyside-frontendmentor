<template>
  <footer>
    <div class="container text-center p-5">
      <a
        href="#"
        class="fs-1 fw-bold"
        style="color: var(--clr-dark-desaturated-cyan)"
        >sunnyside</a
      >

      <ul class="d-flex justify-content-center gap-5 my-3">
        <li><a href="#">About</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Projects</a></li>
      </ul>

      <ul class="d-flex justify-content-center gap-4">
        <li>
          <a href="#"><img src="/images/icon-facebook.svg" alt="" /></a>
        </li>

        <li>
          <a href="#"><img src="/images/icon-instagram.svg" alt="" /></a>
        </li>

        <li>
          <a href="#"><img src="/images/icon-twitter.svg" alt="" /></a>
        </li>

        <li>
          <a href="#"><img src="/images/icon-pinterest.svg" alt="" /></a>
        </li>
      </ul>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style>
footer {
  background-color: var(--clr-dark-moderate-cyan);
}

footer li a {
  color: var(--clr-dark-desaturated-cyan);
}
</style>