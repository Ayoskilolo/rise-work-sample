<script setup lang="ts">
const reviews = [
  {
    name: 'Lade',
    review: 'I don’t want to invest in separate stocks because I’m not a financial expert and I would rather trust my money in the hands of people like Rise who are skilled and knowledgeable.',
    icon: '/girl.jpeg',
    style: "background-image: url('/girl.jpeg')"
  },
  {
    name: 'Jesse',
    review: 'I don’t want to invest in separate stocks because I’m not a financial expert and I would rather trust my money in the hands of people like Rise who are skilled and knowledgeable.',
    icon: '/boy.jpeg',
    style: "background-image: url('/boy.jpeg')"
  },
  {
    name: 'Raye',
    review: 'I chose Rise because of its leadership, wealth of knowledge and the people who support them. I invest with Rise in order to protect my savings and investment from being depleted by devaluation and inflation that’s at an all-time high in Nigeria.',
    icon: '/boy.jpeg',
    style: "background-image: url('/boy.jpeg')"
  },
]
</script>

<template>
  <section>
    <div class="center info">
      <h2>
        From The People Who Use Rise
      </h2>
      <p>
        <span class="line-break-block">Our mission at Risevest is to empower more people just like you
          to achieve your personal financial goals.</span>
      </p>
    </div>

    <Vue3Marquee :pauseOnHover="true" :duration="60" style="height: max-content; margin-bottom: 3rem;">
      <div id="reviewCard" v-for="review in reviews" :key="review">
        <p>
          {{ review.review }}
        </p>

        <div style="display: flex; align-items: center; gap:1rem">
          <div :style="review.style" class="customerPhoto"></div>
          <!-- <img :src="review.icon" alt="" class="customerPhoto" /> -->
          <p>{{ review.name }}</p>

        </div>
      </div>
    </Vue3Marquee>
  </section>
</template>

<style scoped>
section {
  padding: 3rem 0;
}

h2 {
  color: #40BBC3;
  font-family: Tomato Grotesk;
  font-weight: normal;
  margin-bottom: 1rem;
}

p {
  font-size: 1rem;
  margin: 0;
  padding: 0;
}

.info {
  margin-bottom: rem;
  padding: 1rem;
  text-align: center;
}

#reviewCard {
  border-radius: 10px;
  border: 1px solid #ECFEFE;
  height: 200px;
  width: 400px;
  margin: 0.4rem;
  margin-right: 0.5rem;
  padding: 2rem;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  box-shadow: 0px 0px 1em rgba(64, 187, 195, 0.15)
}

.customerPhoto {
  border-radius: 50%;
  width: 50px;
  height: 50px;
  background: transparent no-repeat top;
  background-size: cover;
  behavior: url(PIE.htc);
}

@media (max-width: 1024px) {

  h2 {
    line-height: 40px;
  }

}
</style>
