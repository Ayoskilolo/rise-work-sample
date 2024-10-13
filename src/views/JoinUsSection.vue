<script setup lang="ts">
import { Icon } from '@iconify/vue';
</script>

<template>
  <section>
    <div id="greenBackground">
      <div class="download">
        <p style="color: #07969E;">Download The Rise App</p>
        <h2>
          <span class="line-break-block">Join our 100,000 users investing </span>
          <span class="line-break-block"> and setting long term goals!</span>
        </h2>
        <p>Dollar investments that help you grow.</p>
        <div class="buttons">
          <div class="button">
            <Icon icon="ic:baseline-apple" style="font-size: 45px;" />
            <span>
              <span class="line-break-block">Download on the </span>
              <span class="bold">App Store</span>
            </span>
          </div>
          <div class="button">
            <Icon icon="mage:playstore" style="font-size: 40px;" />
            <span>
              <span class="line-break-block">Download on the</span>
              <span class="bold line-break-block">Play Store</span>
            </span>
          </div>
        </div>
      </div>

      <img src="/Phone.png" alt="" class="joinUsImg" />
    </div>
  </section>
</template>

<style scoped>
section {
  height: 50vh;
  display: flex;
  margin-top: 3rem 8rem;
  align-items: center;
}

h2 {
  padding: 0;
  margin: 0;
}

#greenBackground {
  height: 80%;
  width: 100%;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: space-around;
  color: #2D2D2D;
  background-color: #ECFEFE;
  border-radius: 50px;
}

.download {
  margin: 1.5rem 0;
  padding: 0;
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

.joinUsImg {
  align-items: flex-end;
}

@media (max-width: 1024px) {
  section {
    height: auto;
    margin-bottom: 3rem;
  }

  #greenBackground {
    flex-direction: column;
  }

  .download {
    text-align: center;
  }

  .buttons {
    justify-content: center;
  }
}
</style>
