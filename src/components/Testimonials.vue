<template>
  <section class="testimonials mb-5">
    <div class="container row flex-column flex-md-row justify-content-center align-items-center mx-auto">
      <h1 class="text-center my-5 text-uppercase fs-2">Client testimonials</h1>

      <div v-for="data in datas" :key="data.id" class="col mb-3 mb-md-0" :id="data.id">
        <div class="client-1 text-center d-flex flex-column gap-3 align-items-center">
          <img class="rounded-circle" :src="data.img" :alt="data.name" style="width: 100px">

          <p>{{data.text}}</p>

          <div class="info-person">
            <p class="name-person">{{data.name}}</p>
            <span class="job">{{data.job}}</span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      datas: [
        {
          img: "/images/image-emily.jpg", 
          text: "We put our trust in Sunnyside and they delivered, making sure our needs were met and deadlines were always hit.",
          name: "Emily R.", job: "Marketing Director", id: 1
        },

        {
          img: "/images/image-thomas.jpg", 
          text: "Sunnyside's enthusiasm coupled with their keen interest in our brand's success made it a satisfying and enjoyable experience.",
          name: "Thomas R.", job: "Chief Operating Officer", id: 2
        },

        {
          img: "/images/image-jennie.jpg", 
          text: "Incredible end result! Our sales increased over 400% when we worked with Sunnyside. Highly recommended!",
          name: "Jennie F.", job: "Business Owner", id: 3
        }
      ]
    }
  }
};
</script>

<style>
.testimonials > .container > h1 {
  color: var(--grayish-blue);
  font-family: var(--font-secondary);
}

.name-person {
  font-family: var(--font-secondary);
  font-weight: 900;
}

.job {
  color: var(--grayish-blue);
}
</style>