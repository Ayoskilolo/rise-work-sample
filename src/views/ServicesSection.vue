<script setup lang="ts">
import CallToAction from '../components/CallToAction.vue';
</script>

<template>
  <section id="invest" class="straighten">
    <div class="card-text">
      <h3>Invest your money in dollars</h3>
      <p>
        <span class="line-break-block"> By holding your investments in a stable</span>
        <span class="line-break-block">currency, your money grows more over</span>
        <span class="line-break-block">time and retains its value better.</span>
      </p>
      <CallToAction message="Start Investing Now" />
    </div>

    <img src="/service1.png" />
  </section>

  <section class="reverse  straighten" id="choose">
    <div class="card-text">
      <h3>Choose what's best for you</h3>
      <p>
        <span class="line-break-block">Unlike other platforms, Rise lets you pick between</span>
        <span class="line-break-block"> stocks, US real estate and fixed income, according to</span>
        <span class="line-break-block">your risk appetite. That way you can spread your risk and</span>
        <span class="line-break-block">tap into different investments all in one place.</span>
      </p>
      <CallToAction message="Start Investing Now" />
    </div>

    <img src="/service2.png" />
  </section>

  <section class="straighten">
    <div class="card-text">
      <h3>Set goals and reach them</h3>
      <p>
        <span class="line-break-block">You can invest towards a goal on Rise--retirement, higher</span>
        <span class="line-break-block">education, save for your home or travel budgets. Or create</span>
        <span class="line-break-block">a goal of your own and invest periodically to achieve them.</span>
      </p>
      <CallToAction message="Start Investing Now" />
    </div>

    <img src="/service3.png" />
  </section>

  <section class="reverse hide">
    <div>
      <h3>We remember so you don't have to</h3>
      <p>
        <span class="line-break-block">Our Auto-invest feature makes it easy to stay consistent,</span>
        <span class="line-break-block">even when you forget. Set a funding amount, frequency</span>
        <span class="line-break-block">and payment method and Rise will automatically fund</span>
        <span class="line-break-block">your investment, on schedule.</span>
      </p>
      <CallToAction message="Start Investing Now" />
    </div>

    <img src="/service4.png" />
  </section>
</template>

<style scoped>
section {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 3rem;
  margin: 0;
}

.reverse {
  flex-direction: row-reverse;
}

h3 {
  font-size: 32px;
  padding: 0;
  margin: 0;
}

img {
  transform: scale(1.2);
}

@media (max-width: 1024px) {

  section {
    margin-bottom: 3rem;
  }

  .straighten {
    flex-direction: column-reverse;
    justify-content: center;
  }

  .card-text {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
  }

  .hide {
    display: none;
  }

  img {
    height: 250px;
    box-shadow: inset 0px -3rem #A0DDE2CC;
    margin-bottom: 5rem;
  }
}
</style>
