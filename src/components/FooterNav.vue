<script setup lang="ts">
import { Icon } from '@iconify/vue';
</script>

<template>
  <footer>
    <nav>
      <ul>
        <li class="top logo"><img src="/logo.svg"></li>
        <li>About Us</li>
        <li>Career</li>
        <li>FAQs</li>
        <li>Contact Info</li>
        <li>Press</li>
        <li>Rise Impact</li>
      </ul>

      <ul>
        <li class="top">Explore</li>
        <li>
          Investment Club
          <Icon icon="material-symbols-light:arrow-outward-rounded" style="font-size: 1.2rem;" />
        </li>
        <li>
          <a href="https://risevest.com/blog">Blog</a>
          <Icon icon="material-symbols-light:arrow-outward-rounded" style="font-size: 1.2rem;" />
        </li>
      </ul>

      <ul>
        <li class="top">Products</li>
        <li>Rise Apps</li>
        <li>Wallets</li>
        <li>Asset Classes</li>
      </ul>

      <ul>
        <li class="top">Contact Us</li>
        <li>
          <a href="tel:+2348187147405">0818 714 7405</a>
          <Icon icon="material-symbols-light:arrow-outward-rounded" style="font-size: 1.2rem;" />
        </li>
        <li>
          <a href="mailto:hello@rise.capital">hello@rise.capital</a>
          <Icon icon="material-symbols-light:arrow-outward-rounded" style="font-size: 1.2rem;" />
        </li>
        <li>
          Newsletter
          <Icon icon="material-symbols-light:arrow-outward-rounded" style="font-size: 1.2rem;" />
        </li>
        <li>
          <a href="https://www.instagram.com/rise.vest">Instagram</a>
          <Icon icon="material-symbols-light:arrow-outward-rounded" style="font-size: 1.2rem;" />
        </li>
        <li>
          <a href="https://x.com/risevest">Twitter</a>
          <Icon icon="material-symbols-light:arrow-outward-rounded" style="font-size: 1.2rem;" />
        </li>
      </ul>
    </nav>
  </footer>
</template>

<style scoped>
footer {
  margin: 0;
  padding: 0 7%;
}

nav {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  justify-content: space-between;
  height: auto;
  width: auto;
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.top {
  margin-bottom: 2rem;
  font-weight: bold;
  font-size: 1.2rem;
  font-family: Tomato Grotesk;
  font-weight: normal;
}

.logo {
  /* filter: grayscale(100%); */
  color: black
}

li {
  margin: 1.2rem;
  display: flex;
  gap: 0.3rem;
  align-items: center;
}

@media (max-width: 768px) {
  nav {
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 2rem;
  }
}
</style>
