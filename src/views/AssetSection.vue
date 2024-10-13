<script setup lang="ts">
import { ref } from 'vue';
import CallToAction from '../components/CallToAction.vue';

const recordOfClasses = {
  historicalReturns: '14 % per annum',
  riskLevel: 'Medium'
}

const assetClasses = ref([
  {
    imageURL: '/stocks.png',
    class: 'stocks',
    title: 'Stocks',
    message: 'We help you invest and manage your money by investing in our portfolio of 30 high-growth stocks across the US market with our equity portfolio of power stocks.',
  },
  {
    imageURL: '/realEstate.png',
    class: 'realEstate',
    title: 'Real Estate',
    message: 'Our Real Estate plan is the sweet middle. Best for those who want a balance of good returns and medium risk. This plan invests in rented buildings in the US.'
  },
  {
    imageURL: '/fixedIncome.png',
    class: 'fixedIncome',
    title: 'Fixed Income',
    message: 'A low-risk asset perfect for anyone who wants to protect their money in a secure, appreciating currency, i.e. the dollar. For people who want to protect their hard-earned money from inflation while earning steady returns.'
  }]);


function createCallToActionMessage(assetClass: string) {
  return `Learn how ${assetClass} work`
}
</script>

<template>
  <section>
    <div style="text-align: center; margin-bottom:4rem;">
      <h2>Asset Classes</h2>
      <p>It’s your money, choose where you invest it</p>
    </div>


    <div id="assetClassesCards">
      <div v-for="assetClass of assetClasses" :key="assetClass" id="assetClassesCard">
        <div :class="assetClass.class"></div>
        <img :src="assetClass.imageURL" class="circleBase" />

        <div class="center info">
          <h3>{{ assetClass.title }}</h3>
          <p style="text-align: center; margin-bottom: 0.5rem;"> {{ assetClass.message }}</p>
          <p> <span class="subtitle">Historical returns:</span> {{ recordOfClasses.historicalReturns }}</p>
          <p> <span class="subtitle">Risk Level:</span> {{ recordOfClasses.riskLevel }}</p>
        </div>
        <CallToAction :message="createCallToActionMessage(assetClass.title)" class="callToAction" />

      </div>
    </div>
  </section>
</template>

<style scoped>
section {
  height: max-content;
  margin: 0;
  padding: 3rem 8rem;
}

#assetClassesCards {
  display: flex;
  justify-content: space-around;
  gap: 2rem;
}

p {
  margin: 0;
  padding: 0;
  font-size: 18px;
}

h2 {
  margin: 0;
  padding: 0;
  font-size: 40px;
}

h3 {
  font-size: 25px;
}

#assetClassesCard {
  padding: 0;
  height: auto;
  max-width: 30%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  border: 1.5px solid #919FB533;
  border-radius: 5px;
  text-align: center;
}

.stocks {
  background-color: #FFF4F0;
  width: 100%;
  height: 150px;
}

.realEstate {
  background-color: #F6F2FF;
  width: 100%;
  height: 150px;
}

.fixedIncome {
  background-color: #ECFEFE;
  width: 100%;
  height: 150px;
}

.circleBase {
  margin-top: -50px;
  border: 15px white solid;
  border-radius: 50%;
  width: 100px;
  height: 100px;
  behavior: url(PIE.htc);
  z-index: 1;
}

.subtitle {
  color: #4A5050;
}

.info {
  padding: 0.5rem;
}

.callToAction {
  padding: 1rem;
  margin-top: auto;
}

@media (max-width: 1024px) {
  section {
    padding: 0 5%;
  }

  #assetClassesCards {
    flex-direction: column;
    width: 100%;
  }

  #assetClassesCard {
    max-width: 100%;
  }
}
</style>
