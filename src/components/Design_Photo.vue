<template>
  <div class="row">
    <section class="section-design position-relative col-12 col-sm-0 col-lg-6">
      <div class="text-design text-center p-3 position-absolute bottom-0">
        <h1 class="mb-3">Graphic Design</h1>

        <p>
          Great design makes you memorable. We deliver artwork that underscores
          you brand message and captures potential clients attention.
        </p>
      </div>
    </section>

    <section class="section-photo position-relative col">
      <div class="text-design text-center p-3 position-absolute bottom-0">
        <h1 class="mb-3">Photography</h1>

        <p>
          Increase your credibility by getting the most stunning, high-quality
          photos that improve you business image.
        </p>
      </div>
    </section>
  </div>
</template>

<style>
.section-design {
  background-image: url("/images/mobile/image-graphic-design.jpg");
  color: var(--clr-dark-desaturated-cyan);

  background-size: cover;
  background-position: center;
  height: 100vh;
}

.section-photo {
  background-image: url("/images/mobile/image-photography.jpg");
  color: var(--clr-dark-blue);

  background-size: cover;
  background-position: center;
  height: 100vh;
}

@media only screen and (min-width: 800px) {
    .section-photo {
        background-image: url("/images/desktop/image-photography.jpg")
    }

    .section-design {
        background-image: url("/images/desktop/image-graphic-design.jpg")
    }
}
</style>