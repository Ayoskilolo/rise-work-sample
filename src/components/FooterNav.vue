<script setup lang="ts">
</script>

<template>
  <footer>
    <nav>
      <ul style="flex:grow;">
        <li class="top">Rise</li>
        <li>About Us</li>
        <li>Career</li>
        <li>FAQs</li>
        <li>Contact Info</li>
        <li>Press</li>
        <li>Rise Impact</li>
      </ul>

      <ul>
        <li class="top">Explore</li>
        <li>Investment Club</li>
        <li>Blog</li>
      </ul>

      <ul>
        <li class="top">Products</li>
        <li>Rise Apps</li>
        <li>Wallets</li>
        <li>Asset Classes</li>
      </ul>

      <ul>
        <li class="top">Contact Us</li>
        <li>0818 714 7405</li>
        <li><a href="mailto:hello@rise.capital">hello@rise.capital</a></li>
        <li>Newsletter</li>
        <li>Instagram</li>
        <li>Twitter</li>
      </ul>
    </nav>
  </footer>
</template>

<style scoped>
nav {
  display: flex;
  justify-content: space-between;
  height: 35vh;
  border: 1px solid green;
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.top {
  margin-bottom: 2rem;
}

li {
  margin: 1.2rem
}
</style>
