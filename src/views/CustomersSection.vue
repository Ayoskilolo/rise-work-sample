<script setup lang="ts">
const reviews = [
  {
    name: 'Lade',
    review: 'I don’t want to invest in separate stocks because I’m not a financial expert and I would rather trust my money in the hands of people like Rise who are skilled and knowledgeable.',
    icon: '',
  },
  {
    name: 'Jesse',
    review: 'I don’t want to invest in separate stocks because I’m not a financial expert and I would rather trust my money in the hands of people like Rise who are skilled and knowledgeable.',
    icon: '',
  },
  {
    name: 'Raye',
    review: 'I chose Rise because of its leadership, wealth of knowledge and the people who support them. I invest with Rise in order to protect my savings and investment from being depleted by devaluation and inflation that’s at an all-time high in Nigeria.',
    icon: '',
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
        <span class="line-break-block">Our mission at Risevest is to empower more people just like you</span>
        <span class="line-break-block"> to achieve your personal financial goals.</span>
      </p>
    </div>

    <Vue3Marquee :pauseOnHover="true" :duration="60" style="height: max-content; margin-bottom: 3rem;">
      <div id="reviewCard" v-for="review in reviews" :key="review">
        <p>
          {{ review.review }}
        </p>

        <div>
          <img :src="review.icon" alt="">
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
}

p {
  font-size: 18px;
  margin: 0;
  padding: 0;
}

.info {
  margin-bottom: 3rem;
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
  box-shadow: 0px 0px 1em rgba(64, 187, 195, 0.15)
}
</style>
