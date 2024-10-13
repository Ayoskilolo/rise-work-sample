<script setup lang="ts">
import { Icon } from '@iconify/vue';
</script>

<template>
  <header>
    <div>
      <img src="/logo.svg">
    </div>

    <div class="nav">
      <span>Home</span>
      <span class="arrow">
        Products
        <Icon icon="material-symbols-light:arrow-downward-alt" style="font-size: 25px;" />
      </span>
      <span>Investment Club</span>
      <span>Blog</span>
      <span>About Us</span>
      <span>FAQs</span>
    </div>

    <div class="nav-mobile">
      <Icon icon="ci:hamburger-lg" style="font-size: 25px;" />
    </div>
  </header>
</template>

<style scoped>
header {
  display: flex;
  align-items: center;
  justify-content: space-around;
  color: #07969E;
  font-weight: 200;
  padding: 2rem;
  font-family: Tomato Grotesk;
}

.arrow {
  display: flex;
  align-items: center;
}

.nav {
  display: flex;
  gap: 2.5rem;
}

.nav-mobile {
  display: none;
}

@media (max-width: 1024px) {
  header {
    justify-content: space-between;
    margin-bottom: 3rem;
  }

  .nav {
    display: none;
  }

  .nav-mobile {
    display: block;
  }
}
</style>
