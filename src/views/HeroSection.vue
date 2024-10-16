<script setup lang="ts">
import { Icon } from '@iconify/vue';
</script>

<template>
  <section>
    <div class="heroText">
      <div>
        <h2>
          <span id="topline">Dollar investments</span>
          <span id="bottomline"> that help you grow</span>
        </h2>
        <p>
          <span id="quality">We put your money in high quality assets that help you build wealth and achieve your
            financial goals.</span>
        </p>

        <div class="buttons">
          <a class="button" href="https://click.risevest.com/gb0g/84fr8qjl?af_qr=c">
            <Icon icon="ic:baseline-apple" style="font-size: 45px;" />
            <span>
              <span class="line-break-block">Download on the</span>
              <span class="bold">App Store</span>
            </span>
          </a>
          <a class="button" href="https://click.risevest.com/gb0g/84fr8qjl?af_qr=c">
            <Icon icon="mage:playstore" style="font-size: 40px;" />
            <span>
              <span class="line-break-block">Download on the</span>
              <span class="bold line-break-block">Play Store</span>
            </span>
          </a>
        </div>
      </div>

      <div class="appPreview">
      </div>
    </div>

    <h3 id="supportedBy"> We are supported by:</h3>
    <div class="heroPartners">
      <img src="/arm-logo.png" alt="ARM Trustees Logo" width="50px">
      <img src="/techstars-logo.png" alt="Techstars Logo" width="50px">
      <img src="/western-union-logo.png" alt="Western Union Logo" width="50px">
      <img src="/ventures-logo.png" alt="Ventures Capital Logo" width="50px">
    </div>
  </section>

</template>

<style scoped>
section {
  display: flex;
  flex-direction: column;
  height: 100svh;
}

.heroText {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex: 1;
  padding: 1.5rem;
}

h2 {
  font-family: Tomato Grotesk;
  font-weight: bolder;
  font-size: 4rem;
  line-height: 40px;
  color: #07969E;
  margin: 0;
}

#topline::after,
#bottomline::after {
  content: "\A";
  white-space: pre;
  display: block;
}

p {
  line-height: 15px;
  margin: 0;
  padding: 0;
  font-weight: light;
  color: #4A5050;
}

#quality::after,
#wealth::after {
  content: "\A";
  white-space: pre;
  display: block;
}

#quality {
  line-height: 20px;
  text-align: center;
}

#supportedBy {
  display: none;
}

.heroPartners {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 1rem;
  filter: grayscale(90%);
}

img {
  width: 200px;
}

.appPreview {
  height: 70%;
  width: 30%;
  background-image: url('/appPreview.png');
  background-position: center;
  background-size: contain;
  background-repeat: no-repeat;
}

.buttons {
  height: max-content;
  display: flex;
  gap: 1rem;
  align-items: center;
  justify-content: start;
}

.button {
  display: flex;
  height: 100%;
  border-radius: 10px;
  background-color: #2D2D2D;
  color: #FFFFFF;
  padding: 8px 8px;
}

span.button {
  margin: 0;
  padding: 0;
}

.bold {
  font-weight: bold;
}

@media (max-width: 1024px) {
  .heroText {
    padding: 0;
    margin: 0;
    flex-direction: column;
    gap: 4rem;
  }

  .heroPartners {
    justify-content: space-evenly;
    margin-bottom: 5rem;
  }

  .appPreview {
    height: 100%;
    width: 100%;
    background-image: url('/Phone2.png');
  }

  h2 {
    font-size: 2.2rem;
    line-height: 20px;
    text-align: center;
  }


  .buttons {
    justify-content: center;
  }

  #supportedBy {
    color: grey;
    display: block;
    font-size: 1.5rem;
  }

  img {
    width: 100px;
  }
}

@media (max-width: 764px) {
  img {
    width: 50px;
  }
}
</style>
